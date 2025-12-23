![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## Optimization of hyperparameters by the Genetech algorithm

В данной задаче реализован *генетический алгоритм* для оптимизации гиперпараметров нескольких моделей, выбрана лучшая модель по точности.

**Генетический алгоритм** — это эвристический алгоритм поиска, используемый для решения задач оптимизации и моделирования путём случайного подбора, комбинирования и вариации искомых параметров с использованием механизмов, аналогичных естественному отбору в природе.

Корректно проведена предобработка данных (*train/test split, стандартизация*). Также преобразованы данные под различные архитектуры. Реализованы ключевые элементы генетического алгоритма: *создание популяции, вычисление fitness, селекция (турнир), кроссовер, мутация, эволюция поколений*. Есть итоговая визуализация распределения моделей по поколениям, а также вывод лучшей модели и параметров. В финальной части кода представлен вывод.

<div align="center">

*Схема простого генетического алгоритма:*

<img width="663" height="441" alt="image" src="https://github.com/user-attachments/assets/a1ae10c0-1ea8-4640-a490-8d29f134f7c2" />

</div>

<b><b><b>
    
Для отключения ошибок выполните эту часть кода:

    import os
    os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'  # Отключает большинство предупреждений
    
    import tensorflow as tf
    tf.get_logger().setLevel('ERROR')  # Дополнительное отключение логов
    
    import warnings
    warnings.filterwarnings('ignore')

> Использование графических ускорителей необязательно.
