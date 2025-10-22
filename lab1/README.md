# Анализ данных - Лабораторная работа 1

## Описание данных

### Состав показателей и типы данных:
- **column1**: числовой (int64/float64) - описание колонки
- **column2**: категориальный (object) - описание колонки
- **column3**: дата/время (datetime) - описание колонки
- **column4**: логический (bool) - описание колонки

### Подключаемые библиотеки:
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from datetime import datetime
Методы предобработки данных:

#1. Проверка типов данных
df.dtypes - просмотр типов колонок

pd.to_datetime() - преобразование в datetime

astype() - изменение типа данных

2. Обнаружение пропусков
df.isnull().sum() - подсчет пропусков по колонкам

df.dropna() - удаление пропусков

df.fillna() - заполнение пропусков

3. Преобразование типов
Категориальные переменные: pd.Categorical()

Числовые переменные: pd.to_numeric()

Логические переменные: astype('bool')

4. Визуализация
Гистограммы: plt.hist(), df.hist()

Boxplot: sns.boxplot()

Heatmap: sns.heatmap()

Scatter plot: plt.scatter()

Структура проекта
dataset.csv - исходные данные

analysis.ipynb - код анализа и визуализации

README.md - документация

Результаты
В ходе анализа были выявлены [основные находки], построены визуализации распределения данных.

## Полезные команды Git (дополнительно)

Если хотите работать через командную строку:

```bash
# Клонирование репозитория
git clone https://github.com/ваш-username/data_analysis_project.git

# Добавление файлов
git add .

# Коммит изменений
git commit -m "Добавлен анализ данных"

# Отправка на GitHub
git push origin main

