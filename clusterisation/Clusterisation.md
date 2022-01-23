# Методы

В данной работе рассмотрены различные методы кластеризации - k-means, алгоритм агломеративной иерархической кластеризации и OPTICS.

Реализация - https://github.com/ujnomw/neural-networks/blob/master/clusterisation.ipynb

# Датасеты

Вышеописанные методы тестировались на следующих датасетах:

- Линейно разделимые множества
- Линейно разделимые множества, расположенные близко или касающиеся друг друга
- Линейно неразделимое множество (средняя площадь пересечения 10-20%)
- Линейно неразделимое множество (средняя площадь пересечения 50-70%)
- Эталонный датасет Breast Cancer
- Эталонный датасет Wine Quality

![dataset1](images/dataset1.png)
![dataset2](images/dataset2.png)
![dataset3](images/dataset3.png)
![dataset4](images/dataset4.png)
![dataset_bc](images/dataset_bc.png)
![dataset_wq](images/dataset_wq.png)

# Метрики

Оценка качества кластеризации производилась по следующим метрикам:

- V-мера
- Полнота
- Индекс Фаулкса – Мэллова
- Гомогенность

# Результаты

## k-means

### Евклидова метрика

![dataset1](images/kmeans_euc_1.png)
![dataset2](images/kmeans_euc_2.png)
![dataset3](images/kmeans_euc_3.png)
![dataset4](images/kmeans_euc_4.png)
![dataset_bc](images/kmeans_euc_bc.png)
![dataset_wq](images/kmeans_euc_wq.png)

|               | V-mesure | Completeness | Fowlkes-Mallow | Homogenity |
| :------------ | -------: | -----------: | -------------: | ---------: |
| 1             |        1 |            1 |              1 |          1 |
| 2             | 0.697264 |     0.698022 |       0.735169 |   0.696509 |
| 3             | 0.317407 |     0.320007 |       0.396553 |   0.314848 |
| 4             |  0.08401 |    0.0843068 |       0.239744 |  0.0837153 |
| breast cancer | 0.464793 |     0.516809 |       0.791517 |   0.422291 |
| wine quality  | 0.428757 |     0.428701 |       0.583537 |   0.428812 |

### Манхеттенская метрика

![dataset1](images/kmeans_manh_1.png)
![dataset2](images/kmeans_manh_2.png)
![dataset3](images/kmeans_manh_3.png)
![dataset4](images/kmeans_manh_4.png)
![dataset_bc](images/kmeans_manh_bc.png)
![dataset_wq](images/kmeans_manh_wq.png)

|               |  V-mesure | Completeness | Fowlkes-Mallow | Homogenity |
| :------------ | --------: | -----------: | -------------: | ---------: |
| 1             |         1 |            1 |              1 |          1 |
| 2             |  0.668319 |     0.668937 |       0.688112 |   0.667702 |
| 3             |  0.338049 |     0.339195 |       0.415465 |    0.33691 |
| 4             | 0.0870521 |    0.0876989 |       0.242695 |  0.0864148 |
| breast cancer |  0.456708 |     0.510052 |       0.788211 |   0.413465 |
| wine quality  |  0.431543 |     0.431385 |       0.585935 |   0.431701 |

## Алгоритм агломеративной иерархической кластеризации

### Евклидова метрика

![dataset1](images/agglo_euc_1.png)
![dataset2](images/agglo_euc_2.png)
![dataset3](images/agglo_euc_3.png)
![dataset4](images/agglo_euc_4.png)
![dataset_bc](images/agglo_euc_bc.png)
![dataset_wq](images/agglo_euc_wq.png)

|               |  V-mesure | Completeness | Fowlkes-Mallow | Homogenity |
| :------------ | --------: | -----------: | -------------: | ---------: |
| 1             |         1 |            1 |              1 |          1 |
| 2             |  0.675832 |     0.678153 |       0.709681 |   0.673526 |
| 3             |  0.321083 |     0.323531 |       0.384739 |   0.318672 |
| 4             | 0.0830093 |    0.0852188 |       0.246371 |  0.0809116 |
| breast cancer |  0.319082 |     0.407601 |       0.739228 |    0.26215 |
| wine quality  |  0.416077 |     0.416293 |       0.582122 |   0.415861 |

### Манхеттенская метрика

![dataset1](images/agglo_manh_1.png)
![dataset2](images/agglo_manh_2.png)
![dataset3](images/agglo_manh_3.png)
![dataset4](images/agglo_manh_4.png)
![dataset_bc](images/agglo_manh_bc.png)
![dataset_wq](images/agglo_manh_wq.png)

|               |  V-mesure | Completeness | Fowlkes-Mallow | Homogenity |
| :------------ | --------: | -----------: | -------------: | ---------: |
| 1             |         1 |            1 |              1 |          1 |
| 2             |  0.661681 |     0.673164 |       0.673158 |   0.650584 |
| 3             |  0.328866 |      0.33839 |       0.414054 |   0.319864 |
| 4             | 0.0565259 |    0.0654418 |       0.273425 |  0.0497481 |
| breast cancer | 0.0880967 |     0.235139 |       0.721494 |  0.0542019 |
| wine quality  |  0.442275 |     0.448047 |       0.589682 |    0.43665 |

## OPTICS

### Евклидова метрика

![dataset1](images/optics_euc_1.png)
![dataset2](images/optics_euc_2.png)
![dataset3](images/optics_euc_3.png)
![dataset4](images/optics_euc_4.png)
![dataset_bc](images/optics_euc_bc.png)
![dataset_wq](images/optics_euc_wq.png)

|               | V-mesure | Completeness | Fowlkes-Mallow | Homogenity |
| :------------ | -------: | -----------: | -------------: | ---------: |
| 1             |        1 |            1 |              1 |          1 |
| 2             | 0.356688 |     0.389988 |       0.346776 |   0.328627 |
| 3             | 0.217932 |     0.179928 |       0.225498 |   0.276288 |
| 4             | 0.249568 |     0.174175 |      0.0962486 |   0.440045 |
| breast cancer | 0.154971 |     0.117049 |       0.493887 |   0.229242 |
| wine quality  | 0.276606 |     0.180435 |       0.152288 |   0.592305 |

### Манхеттенская метрика

![dataset1](images/optics_manh_1.png)
![dataset2](images/optics_manh_2.png)
![dataset3](images/optics_manh_3.png)
![dataset4](images/optics_manh_4.png)
![dataset_bc](images/optics_manh_bc.png)
![dataset_wq](images/optics_manh_wq.png)

|               | V-mesure | Completeness | Fowlkes-Mallow | Homogenity |
| :------------ | -------: | -----------: | -------------: | ---------: |
| 1             |        1 |            1 |              1 |          1 |
| 2             | 0.358768 |     0.389889 |       0.356059 |   0.332248 |
| 3             | 0.203824 |     0.171729 |       0.232271 |   0.250673 |
| 4             | 0.243216 |     0.170108 |      0.0922051 |   0.426524 |
| breast cancer | 0.130749 |     0.154482 |       0.659543 |   0.113337 |
| wine quality  | 0.303906 |     0.198218 |       0.159531 |   0.651029 |
