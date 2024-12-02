# Задание 4: PCA, t-SNE, UMAP

## [1] Генерация двумерных датасетов
- Создать датасеты `df_a` размерностей 4x4, 16x16, 256x256.
- В каждой строке начиная с колонки `y (=x)` значения следующих `(a/2)` ячеек равны `1`. Остальные ячейки равны `0`.
- Визуализировать эти датасеты в пространстве X-Y.

## [2] Метод главных компонент (PCA)
Для каждого датасета `df_a` выполнить визуализацию:
1. Scree plot.
2. Отображения отдельных объектов-строк в двумерных пространствах первых компонент от 1 до `a` (где `a` от 4 до 8):
   - Без отображения старых векторов-переменных.
   - С отображением старых векторов-переменных.
3. Отображения отдельных объектов-строк в двумерных пространствах первых компонент от `c` до `c+a` (где `c` ≥ 129, `a` от 4 до 8):
   - Без отображения старых векторов-переменных.
   - С отображением старых векторов-переменных.

## [3] Методы UMAP, PaCMAP и t-SNE
Для каждого датасета `df_a` выполнить:
1. Визуализацию проекций с нескольких случайных стартов.
2. Визуализацию после предварительного применения PCA.

## [4] Генерация датасета `df_256v`
1. Используя `make_blobs`, сгенерировать новый датасет `df_256v` на основе:
   - Номеров строк (`x`), столбцов (`y`) и значений (`0`, `1`) ячеек `df_256`.
   - Для каждой точки с центром `(x, y)` и дисперсией `d` (в диапазоне от 5 до 20) сформировать по 10 случайных точек класса `1` или `0`.

## [5] Анализ датасета `df_256v` с помощью PCA
Выполнить визуализацию аналогично пункту [2]:
1. Scree plot.
2. Отображения в двумерных пространствах для первых компонент.

## [6] Методы UMAP, PaCMAP и t-SNE для `df_256v`
Повторить шаги из пункта [3].

## [7] Анализ датасета с Kaggle
1. Выбрать датасет с ≥10 переменными, ≥10000 объектами и несколькими классами.
2. Повторить шаги из задания 1:
   - Определение ключевых характеристик датасета.
   - Корреляционный анализ.
   - Визуализация всех пар переменных.

## [8] Анализ Kaggle-датасета с помощью PCA
1. Выполнить визуализацию аналогично пункту [2].
2. Определить количество необходимых компонент для регрессионной модели:
   - Метод Кайзера.
   - Метод сломанной трости.

## [9] Методы UMAP, PaCMAP и t-SNE для Kaggle-датасета
Повторить шаги из пункта [3].

---

## Полезные ссылки
- [UMAP Documentation](https://umap-learn.readthedocs.io/en/latest/)
- [PaCMAP GitHub](https://github.com/YingfanWang/PaCMAP)