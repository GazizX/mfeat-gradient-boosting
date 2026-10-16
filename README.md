# Tree-Based Classification on UCI mfeat-fac

[English](#english) | [Русский](#русский)

## English

A multiclass classification experiment on the UCI Multiple Features handwritten-digit dataset. It compares decision trees, random forests, and gradient boosting, with a focus on validation-based model selection and feature importance.

### Notebook

- `mfeat_gradient_boosting.ipynb` — data preparation, model comparisons, plots, and held-out evaluation.

### Dataset

The notebook downloads the `mfeat-fac` feature file from the [UCI Multiple Features dataset](https://archive.ics.uci.edu/dataset/72/multiple+features). It contains 2,000 examples of digits 0–9 represented by 216 numerical features.

### Experiments

- Stratified train/validation/test split (60% / 20% / 20%)
- Decision-tree depth and split-size comparison
- Random-forest estimator count, feature sampling, and depth comparison
- GradientBoostingClassifier performance across boosting stages
- Feature-importance analysis and random-forest evaluation on selected feature subsets
- Test accuracy and macro F1 reporting

### Run

```bash
python -m pip install numpy pandas matplotlib scikit-learn jupyter
```

Open `mfeat_gradient_boosting.ipynb` in Jupyter and run the cells from top to bottom. Internet access is required to download the dataset from UCI.

## Русский

Эксперимент по многоклассовой классификации на наборе рукописных цифр UCI Multiple Features. Сравниваются решающие деревья, случайный лес и градиентный бустинг; подбор выполняется по валидационной выборке, отдельно анализируется важность признаков.

### Ноутбук

- `mfeat_gradient_boosting.ipynb` — подготовка данных, сравнение моделей, графики и итоговая оценка.

### Данные

Ноутбук скачивает файл признаков `mfeat-fac` из набора [UCI Multiple Features](https://archive.ics.uci.edu/dataset/72/multiple+features). В нём 2 000 примеров цифр 0–9, каждый описан 216 числовыми признаками.

### Эксперименты

- Стратифицированное разбиение train/validation/test (60% / 20% / 20%)
- Сравнение глубины дерева и минимального размера разбиения
- Сравнение числа деревьев, выбора признаков и глубины в Random Forest
- Оценка GradientBoostingClassifier на разных этапах бустинга
- Анализ важности признаков и моделей на разных поднаборах признаков
- Итоговые метрики: accuracy и macro F1 на тестовой выборке

### Запуск

```bash
python -m pip install numpy pandas matplotlib scikit-learn jupyter
```

Откройте `mfeat_gradient_boosting.ipynb` в Jupyter и выполните ячейки по порядку. Для загрузки данных с UCI требуется интернет-соединение.
