# Архитектура

В основе сверточной нейронной сети лежит идея применения слоя фильтров на небольшие участки изображения для выдления характерных признаков изображения (вертикальные, горизонтальные линии например). Последовательное использование подобных слоев приводит к выделению более специфичных признаков, например фары автомобиля.

Дальнейшие слои осуществляют классификацию на основе выделенных признаков.

Архитектура используеммой CNN:

![Screen Shot 2021-06-19 at 22.07.26](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.07.26.png)

# Результаты для CIFAR-10

```text
Train on 37500 samples, validate on 12500 samples
Epoch 1/15
37500/37500 [==============================] - 93s 2ms/sample - loss: 1.8548 - accuracy: 0.3143 - val_loss: 1.5648 - val_accuracy: 0.4381
Epoch 2/15
37500/37500 [==============================] - 94s 2ms/sample - loss: 1.5262 - accuracy: 0.4447 - val_loss: 1.3758 - val_accuracy: 0.5008
Epoch 3/15
37500/37500 [==============================] - 96s 3ms/sample - loss: 1.4006 - accuracy: 0.4958 - val_loss: 1.2906 - val_accuracy: 0.5439
Epoch 4/15
37500/37500 [==============================] - 98s 3ms/sample - loss: 1.3138 - accuracy: 0.5322 - val_loss: 1.2452 - val_accuracy: 0.5584
Epoch 5/15
37500/37500 [==============================] - 98s 3ms/sample - loss: 1.2413 - accuracy: 0.5584 - val_loss: 1.1609 - val_accuracy: 0.5917
Epoch 6/15
37500/37500 [==============================] - 99s 3ms/sample - loss: 1.1831 - accuracy: 0.5814 - val_loss: 1.1113 - val_accuracy: 0.6153
Epoch 7/15
37500/37500 [==============================] - 100s 3ms/sample - loss: 1.1214 - accuracy: 0.6046 - val_loss: 1.0503 - val_accuracy: 0.6360
Epoch 8/15
37500/37500 [==============================] - 100s 3ms/sample - loss: 1.0751 - accuracy: 0.6219 - val_loss: 1.0240 - val_accuracy: 0.6406
Epoch 9/15
37500/37500 [==============================] - 101s 3ms/sample - loss: 1.0310 - accuracy: 0.6375 - val_loss: 0.9847 - val_accuracy: 0.6578
Epoch 10/15
37500/37500 [==============================] - 102s 3ms/sample - loss: 0.9933 - accuracy: 0.6505 - val_loss: 0.9309 - val_accuracy: 0.6731
Epoch 11/15
37500/37500 [==============================] - 103s 3ms/sample - loss: 0.9574 - accuracy: 0.6647 - val_loss: 0.9161 - val_accuracy: 0.6832
Epoch 12/15
37500/37500 [==============================] - 103s 3ms/sample - loss: 0.9279 - accuracy: 0.6756 - val_loss: 0.9161 - val_accuracy: 0.6843
Epoch 13/15
37500/37500 [==============================] - 104s 3ms/sample - loss: 0.9034 - accuracy: 0.6827 - val_loss: 0.8615 - val_accuracy: 0.6993
Epoch 14/15
37500/37500 [==============================] - 105s 3ms/sample - loss: 0.8649 - accuracy: 0.6960 - val_loss: 0.8866 - val_accuracy: 0.6898
Epoch 15/15
37500/37500 [==============================] - 104s 3ms/sample - loss: 0.8453 - accuracy: 0.7011 - val_loss: 0.8326 - val_accuracy: 0.7111

```

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
