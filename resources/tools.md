# Tools (инструменты курса)

Это список инструментов, которые встречаются в семинарах, ДЗ, проекте.
Желательно использовать **uv** как базовый инструмент для окружения и установки зависимостей.

---

## 0) База окружения (обязательно)

- **uv** – менеджер окружения и пакетов (основной инструмент курса).
  Docs: [https://docs.astral.sh/uv/](https://docs.astral.sh/uv/)
- **Python 3.11+**
- **Jupyter** / **JupyterLab** – запуск ноутбуков семинаров.
  [https://jupyter.org/](https://jupyter.org/)

---

## 1) Минимальный стек для большинства семинаров (обычно нужно)

- **NumPy** – базовые массивы и вычисления.
  [https://numpy.org/](https://numpy.org/)
- **Pandas** – табличные данные и EDA.
  [https://pandas.pydata.org/](https://pandas.pydata.org/)
- **Matplotlib** – графики.
  [https://matplotlib.org/](https://matplotlib.org/)
- **scikit-learn** – классические модели, пайплайны, метрики, CV.
  [https://scikit-learn.org/](https://scikit-learn.org/)

---

## 2) Часто полезно (по ситуации)

### Дисбаланс классов и метрики

- **imbalanced-learn** – ресэмплинг и методы под дисбаланс.
  [https://imbalanced-learn.org/](https://imbalanced-learn.org/)

### Бустинг / "сильные" классические модели

- **XGBoost**
  [https://xgboost.readthedocs.io/](https://xgboost.readthedocs.io/)
- **LightGBM**
  [https://lightgbm.readthedocs.io/](https://lightgbm.readthedocs.io/)

### Нейросети (когда дойдём до NN-блока)

- **PyTorch**
  [https://pytorch.org/](https://pytorch.org/)

---

## 3) Интерпретация и диагностика (XAI)

- **SHAP** – универсальные атрибуции (особенно удобен для деревьев, ансамблей и табличных моделей).
  [https://shap.readthedocs.io/](https://shap.readthedocs.io/)
- **LIME** – локальные объяснения (как базовый инструмент).
  [https://github.com/marcotcr/lime](https://github.com/marcotcr/lime)
- **Captum** – интерпретация для моделей на PyTorch.
  [https://captum.ai/](https://captum.ai/)

---

## 4) Дрейф, качество данных, устойчивость к сдвигам

- **Evidently** – отчёты по data drift / quality / мониторинг метрик.
  [https://docs.evidentlyai.com/](https://docs.evidentlyai.com/)
- **Alibi Detect** – детекторы дрейфа/выбросов/аномалий (в т.ч. offline).
  [https://github.com/SeldonIO/alibi-detect](https://github.com/SeldonIO/alibi-detect)

---

## 5) ML Security (только в безопасных учебных постановках)

- **MITRE ATLAS** – база тактик/техник угроз AI/ML (для threat modeling и языка обсуждения рисков).
  [https://atlas.mitre.org/](https://atlas.mitre.org/)
- **Adversarial Robustness Toolbox (ART)** – оценка и защитные меры для ML-систем (учебные кейсы).
  Docs: [https://adversarial-robustness-toolbox.readthedocs.io/](https://adversarial-robustness-toolbox.readthedocs.io/)
  GitHub: [https://github.com/Trusted-AI/adversarial-robustness-toolbox](https://github.com/Trusted-AI/adversarial-robustness-toolbox)

---

## 6) Рекомендуемые "инструменты дисциплины" (если делаете проект серьёзнее)

- **pytest** – минимальные тесты (проверка функций/метрик/препроцессинга).
  [https://docs.pytest.org/](https://docs.pytest.org/)
- **ruff** – быстрый линтер/форматирование (чтобы не тонуть в стиле).
  [https://docs.astral.sh/ruff/](https://docs.astral.sh/ruff/)

---

## 7) Как ставить пакеты (паттерн курса)

Мы используем `uv` и ставим зависимости "по мере необходимости".

Примеры:

- создать окружение: `uv venv`
- поставить базовый стек: `uv pip install numpy pandas matplotlib scikit-learn`
- поставить Jupyter: `uv pip install jupyter` (или `jupyterlab`)

Точные зависимости для конкретного семинара – в `seminars/Sxx/Sxx-brief.md`.
