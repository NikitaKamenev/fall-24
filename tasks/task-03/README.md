# Лабораторная работа №3. Логическая классификация

В рамках лабораторной работы предстоит реализовать алгоритм построения бинарного решающего дерева и сравнить его с эталонной реализацией.

На лекции были рассмотрены следующие алгоритмы:
* алгоритм построения бинарного решающего дерева ID3;
* алгоритм редукции дерева;
* алгоритм бинаризации вещественного признака;

## Задание

1. выбрать датасет для классификации, например на [kaggle](https://www.kaggle.com/datasets?tags=13302-Classification);
   1. датасет должен содержать пропуски;
   2. датасет должен содержать категориальные и количественные признаки;
2. реализовать алгоритм построения дерева ID3 с разными критериями:
   1. критерий Донского;
   2. многоклассовый энтропийный критерий;
3. обучить дерево на выбранном датасете;
4. оценить качество классификации;
5. аналогично 1. - 4. решить задачу регрессии;
6. реализовать алгоритм редукции дерева;
7. сравнить качество классификации и регрессии до и после редукции дерева;
8. сравнить с [эталонной](https://scikit-learn.org/stable/) реализацией бинарного решающего дерева;
    1. сравнить качество работы;
    2. сравнить время работы;
9. подготовить небольшой отчет о проделанной работе.


## Примечание про задачу регрессии

В задаче регрессии в качестве меры неопределенности следует использовать среднеквадратичную ошибку. (см. Лекция 3, слайд 29).