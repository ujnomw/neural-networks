# Архитектура

В основе сверточной нейронной сети лежит идея применения слоя фильтров на небольшие участки изображения для выдления характерных признаков изображения (вертикальные, горизонтальные линии например). Последовательное использование подобных слоев приводит к выделению более специфичных признаков, например фары автомобиля.

Дальнейшие слои осуществляют классификацию на основе выделенных признаков.

Архитектура используеммой CNN:

![Screen Shot 2021-06-19 at 22.07.26](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.07.26.png)

# Результаты для CIFAR-10

Динамика обучения

![Screen Shot 2021-06-19 at 22.07.35](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.07.35.png)

Тестовое множество

![Screen Shot 2021-06-19 at 22.07.45](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.07.45.png)

Обучающие множество

![Screen Shot 2021-06-19 at 22.07.54](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.07.54.png)

# Результаты для CIFAR-10 + vehicles 2

![Screen Shot 2021-06-19 at 22.55.09](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.55.09.png)

![Screen Shot 2021-06-19 at 22.55.17](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.55.17.png)

![Screen Shot 2021-06-19 at 22.55.25](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.55.25.png)

![Screen Shot 2021-06-19 at 22.55.31](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.55.31.png)