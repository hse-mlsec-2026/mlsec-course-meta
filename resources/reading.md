# Reading (что читать по курсу)

Ниже – список материалов, которые помогают разобраться в темах курса.
Структура: **минимум** (что желательно прочитать всем) и **углубление** (по желанию).

---

## 0) Минимум (рекомендуется всем)

### Риск-ориентированная рамка и "ML как часть системы"

- **NIST AI RMF 1.0 (AI Risk Management Framework)** – как думать про риски и доверие к ИИ системно, по жизненному циклу.
  Link: [https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf](https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf)
- **MITRE ATLAS** – "ATT&CK-стиль" база тактик/техник атак на AI/ML-системы (угрозы, кейсы, таксономия).
  Link: [https://atlas.mitre.org/](https://atlas.mitre.org/)

### Данные, протокол проверки, метрики (основа воспроизводимости)

- **scikit-learn User Guide (Model evaluation / Cross-validation / Metrics)** – практическая база по протоколам и метрикам.
  Link: [https://scikit-learn.org/stable/user_guide.html](https://scikit-learn.org/stable/user_guide.html)
- **Статья/гайд по data leakage (утечки данных)** – как утечки возникают и почему ломают проверку.
  (Рекомендуется опираться на разделы про preprocessing, CV в scikit-learn и практики из семинаров курса.)

### Интерпретация и разбор ошибок (как инструмент диагностики)

- **SHAP documentation** – единая рамка атрибуций (почему это работает и как применять).
  Link: [https://shap.readthedocs.io/](https://shap.readthedocs.io/)
- **Captum (PyTorch interpretability)** – атрибуции/интерпретация для нейросетей на PyTorch.
  Link: [https://captum.ai/](https://captum.ai/)

### Сдвиги данных, дрейф, устойчивость (надёжность в ИБ)

- **Evidently AI (Drift и data quality)** – практические метрики/отчёты по дрейфу данных.
  Link: [https://docs.evidentlyai.com/](https://docs.evidentlyai.com/)
- **Alibi Detect (drift / outlier / adversarial detection)** – библиотека для детекторов дрейфа/аномалий.
  Link: [https://github.com/SeldonIO/alibi-detect](https://github.com/SeldonIO/alibi-detect)

### Прикладная ML-security (оценка угроз без "вредных" практик)

- **Adversarial Robustness Toolbox (ART)** – библиотека для оценки/защиты ML-систем (в учебных безопасных постановках).
  Docs: [https://adversarial-robustness-toolbox.readthedocs.io/](https://adversarial-robustness-toolbox.readthedocs.io/)
  GitHub: [https://github.com/Trusted-AI/adversarial-robustness-toolbox](https://github.com/Trusted-AI/adversarial-robustness-toolbox)

---

## 1) Углубление (по темам)

### Adversarial examples / уклоняющиеся воздействия (теория и интуиция)

- Szegedy et al. (2013): *Intriguing properties of neural networks* (классика про adversarial examples).
  Link: [https://arxiv.org/abs/1312.6199](https://arxiv.org/abs/1312.6199)
- Goodfellow et al. (2014): *Explaining and Harnessing Adversarial Examples* (интуиция "почему это возможно").
  Link: [https://arxiv.org/abs/1412.6572](https://arxiv.org/abs/1412.6572)

### Poisoning / data poisoning (отравление данных)

- Biggio et al. (2012): *Poisoning Attacks against Support Vector Machines*.
  Link: [https://arxiv.org/abs/1206.6389](https://arxiv.org/abs/1206.6389)
- Steinhardt et al. (2017): *Certified Defenses for Data Poisoning Attacks*.
  Link: [https://arxiv.org/abs/1706.03691](https://arxiv.org/abs/1706.03691)

### Model stealing / extraction и privacy inference (общее понимание угроз)

- Обзорные материалы по "model extraction / membership inference" (подходы, риски, ограничения).
  (Добавляйте сюда 1-2 ключевые статьи/обзора по мере прохождения соответствующей лекции.)

### Интерпретация (шире SHAP)

- LIME (Ribeiro et al., 2016): *"Why Should I Trust You?"* (локальные объяснения).  
  Link: [https://arxiv.org/abs/1602.04938](https://arxiv.org/abs/1602.04938)

### Про воспроизводимость и инженерную дисциплину эксперимента

- Рекомендации/гайдлайны по экспериментам (фиксировать разбиение, seed, протокол, артефакты).  
  (Опираемся на практики семинаров и требования к отчётам в ДЗ или в проекте.)

---

## 2) Как пользоваться этим списком

- Если не хочется "читать всё": проходите раздел 0) и потом добавляйте по 1-2 материала из раздела 1) на тему, которую берёте в ДЗ/проект.
- В отчётах указывайте, какие источники вы реально использовали.
