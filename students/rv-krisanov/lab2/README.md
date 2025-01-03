# Отчёт по классификации методом K-ближайших соседей (KNN) с использованием окна Парзена

## 1. Датасет
Для задачи классификации был выбран датасет с Kaggle о [рыбах](https://www.kaggle.com/datasets/taweilo/fish-species-sampling-weight-and-height-data).

## 2. Реализация алгоритма с методом окна Парзена
Алгоритм KNN был реализован с использованием метода окна Парзена переменной ширины. В качестве ядра использовано гауссово ядро:

## 3. Подбор параметра \(k\) методом Leave-One-Out
Параметр k был подобран методом скользящего контроля. Каждый элемент данных использовался как тестовый, а остальные для обучения. Этот метод даёт более точную оценку модели без риска переобучения.

Оптимальный диапазон k был выбран между 40 и 60, исходя из графиков эмпирического риска.
![image](https://github.com/user-attachments/assets/c320bc0a-0107-4831-b605-babea448e843)

## 5. График эмпирического риска
График эмпирического риска показывает, как ошибка классификации возрастает с увеличением k. Наилучший результат достигается в диапазоне 40-60, где ошибка минимальна, но затем начинает увеличиваться с ростом k.
![image](https://github.com/user-attachments/assets/732f6133-575a-41d5-9f7d-9f08fbdec93e)

## 6. Сравнение с библиотечной реализацией
- **Accuracy**: Библиотечная реализация из `scikit-learn` показала accuracy **0.9443627450980392**, близкую к результатам собственной реализации (0.9438725490196078).

## 7. Сравнение времени работы
- **Библиотечная реализация KNN (scikit-learn)**: **89 мс**.
- **Собственная реализация с окном Парзена**: **305 мс**.

## 8. Выводы
Была успешно реализована классификация KNN с использованием окна Парзена. Подбор параметра k методом LOO позволил найти оптимальный диапазон k = 40-60.

