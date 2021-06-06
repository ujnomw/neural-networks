# Методы

В данной работе рассмотрены различные методы кластеризации - k-means, алгоритм агломеративной иерархической кластеризации и OPTICS.

Реализация - https://github.com/ujnomw/neural-networks/blob/master/clusterisation.ipynb

# Датасеты

Вышеописанные методы тестировались на следующих датасетах:

* Линейно разделимые множества
* Линейно разделимые множества, расположенные близко или касающиеся друг друга
* Линейно неразделимое множество (средняя площадь пересечения 10-20%)
* Линейно неразделимое множество (средняя площадь пересечения 50-70%)
* Эталонный датасет Breast Cancer
* Эталонный датасет Wine Quality

![Screen Shot 2021-06-06 at 19.51.32](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 19.51.32.png)

![Screen Shot 2021-06-06 at 19.51.44](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 19.51.44.png)

![Screen Shot 2021-06-06 at 19.51.54](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 19.51.54.png)

# Метрики

Оценка качества кластеризации производилась по следующим метрикам:

* V-мера
* Полнота
* Индекс Фаулкса – Мэллова 
* Гомогенность

# Результаты

## k-means

### Евклидова метрика

![Screen Shot 2021-06-06 at 19.51.32](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 19.51.32.png)

![Screen Shot 2021-06-06 at 19.51.44](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 19.51.44.png)

![Screen Shot 2021-06-06 at 19.51.54](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 19.51.54.png)

![Screen Shot 2021-06-06 at 19.58.12](/Users/mgolovatskikh/Library/Application Support/typora-user-images/Screen Shot 2021-06-06 at 19.58.12.png)

### Манхеттенская метрика

![Screen Shot 2021-06-06 at 19.59.21](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 19.59.21.png)

![Screen Shot 2021-06-06 at 19.59.34](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 19.59.34.png)

![Screen Shot 2021-06-06 at 19.59.46](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 19.59.46.png)

## Алгоритм агломеративной иерархической кластеризации

### Евклидова метрика

![Screen Shot 2021-06-06 at 20.06.03](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.06.03.png)

![Screen Shot 2021-06-06 at 20.06.13](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.06.13.png)

![Screen Shot 2021-06-06 at 20.04.56](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.04.56.png)

### Манхеттенская метрика

![Screen Shot 2021-06-06 at 20.06.51](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.06.51.png)

![Screen Shot 2021-06-06 at 20.07.00](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.07.00.png)

![Screen Shot 2021-06-06 at 20.07.13](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.07.13.png)

## OPTICS

### Евклидова метрика

![Screen Shot 2021-06-06 at 20.07.59](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.07.59.png)

![Screen Shot 2021-06-06 at 20.08.07](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.08.07.png)

![Screen Shot 2021-06-06 at 20.08.14](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.08.14.png)

### Манхеттенская метрика

![Screen Shot 2021-06-06 at 20.08.58](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.08.58.png)

![Screen Shot 2021-06-06 at 20.09.11](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.09.11.png)

![Screen Shot 2021-06-06 at 20.09.17](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-06 at 20.09.17.png)

