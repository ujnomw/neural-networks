# Архитектура

В основе сверточной нейронной сети лежит идея применения слоя фильтров на небольшие участки изображения для выдления характерных признаков изображения (вертикальные, горизонтальные линии например). Последовательное использование подобных слоев приводит к выделению более специфичных признаков, например фары автомобиля.

Дальнейшие слои осуществляют классификацию на основе выделенных признаков.

Архитектура - https://learnopencv.com/image-classification-using-convolutional-neural-networks-in-keras/

Архитектура используеммой CNN:

```text
Model: "sequential_28"
_________________________________________________________________
Layer (type)                 Output Shape              Param #
=================================================================
conv2d_38 (Conv2D)           (None, 30, 30, 32)        896
_________________________________________________________________
conv2d_39 (Conv2D)           (None, 28, 28, 32)        9248
_________________________________________________________________
max_pooling2d_21 (MaxPooling (None, 14, 14, 32)        0
_________________________________________________________________
dropout_27 (Dropout)         (None, 14, 14, 32)        0
_________________________________________________________________
conv2d_40 (Conv2D)           (None, 14, 14, 64)        18496
_________________________________________________________________
conv2d_41 (Conv2D)           (None, 12, 12, 64)        36928
_________________________________________________________________
max_pooling2d_22 (MaxPooling (None, 6, 6, 64)          0
_________________________________________________________________
dropout_28 (Dropout)         (None, 6, 6, 64)          0
_________________________________________________________________
conv2d_42 (Conv2D)           (None, 6, 6, 64)          36928
_________________________________________________________________
conv2d_43 (Conv2D)           (None, 4, 4, 64)          36928
_________________________________________________________________
max_pooling2d_23 (MaxPooling (None, 2, 2, 64)          0
_________________________________________________________________
dropout_29 (Dropout)         (None, 2, 2, 64)          0
_________________________________________________________________
flatten_10 (Flatten)         (None, 256)               0
_________________________________________________________________
dense_49 (Dense)             (None, 512)               131584
_________________________________________________________________
dropout_30 (Dropout)         (None, 512)               0
_________________________________________________________________
dense_50 (Dense)             (None, 10)                5130
=================================================================
Total params: 276,138
Trainable params: 276,138
Non-trainable params: 0
_________________________________________________________________
```

# Результаты для CIFAR-10

Динамика обучения

![acc](images/cnn_acc.png)
![loss](images/cnn_loss.png)

Тестовое множество

```text
test:
              precision    recall  f1-score   support

           0       0.81      0.85      0.83      1000
           1       0.86      0.95      0.90      1000
           2       0.72      0.71      0.72      1000
           3       0.72      0.62      0.67      1000
           4       0.84      0.72      0.78      1000
           5       0.74      0.75      0.75      1000
           6       0.83      0.86      0.85      1000
           7       0.82      0.88      0.85      1000
           8       0.86      0.90      0.88      1000
           9       0.89      0.87      0.88      1000

    accuracy                           0.81     10000
   macro avg       0.81      0.81      0.81     10000
weighted avg       0.81      0.81      0.81     10000
```

![conf_test](images/cnn_confusion_test.png)

Обучающие множество

```text
train:
              precision    recall  f1-score   support

           0       0.93      0.95      0.94      3763
           1       0.96      0.99      0.97      3754
           2       0.90      0.89      0.90      3708
           3       0.88      0.81      0.84      3747
           4       0.96      0.87      0.91      3751
           5       0.86      0.86      0.86      3767
           6       0.93      0.96      0.94      3757
           7       0.91      0.97      0.94      3744
           8       0.95      0.98      0.97      3765
           9       0.97      0.97      0.97      3744

    accuracy                           0.93     37500
   macro avg       0.93      0.93      0.93     37500
weighted avg       0.93      0.93      0.93     37500
```

![conf_train](images/cnn_confusion_train.png)

Аналогичная архитектура была использованна в [данной работе](https://learnopencv.com/image-classification-using-convolutional-neural-networks-in-keras/). Полученные результаты незначительно превосходят вышеупомянутые.

# Результаты для CIFAR-10 + vehicles 2

![Screen Shot 2021-06-19 at 22.55.09](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.55.09.png)

![Screen Shot 2021-06-19 at 22.55.17](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.55.17.png)

![Screen Shot 2021-06-19 at 22.55.25](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.55.25.png)

![Screen Shot 2021-06-19 at 22.55.31](/Users/mgolovatskikh/Desktop/Screen Shot 2021-06-19 at 22.55.31.png)