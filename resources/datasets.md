# Datasets (датасеты курса)

Этот файл – реестр датасетов, которые используются в ДЗ или проекте, и правила работы с ними.
**Не храним** крупные датасеты в git: в репозитории остаются только ссылки, инструкции скачивания и/или генераторы синтетики.
См. также: `policies/data-policy.md`.

---

## 1) Правила (коротко)

- Не коммитьте в репозиторий: CSV/Parquet/дампы/модели/большие бинарники.
- В репозитории должно быть воспроизводимо:
  - ссылка на источник,
  - и/или скрипт/ноутбук `download_*`,
  - и/или генератор синтетики.
- Если датасет требует регистрации/принятия условий – это нормально, но тогда в инструкции явно пишем шаги.

---

## 2) Возможные публичные датасеты для проекта (варианты по трекам)

### Трек A / "табличный" / сетевой трафик (IDS/NIDS)

- [CIC-IDS2017 (UNB CIC)](https://www.unb.ca/cic/datasets/ids-2017.html) – трафик + разметка, есть CSV по потокам.
- [UNSW-NB15 (UNSW)](https://research.unsw.edu.au/projects/unsw-nb15-dataset) – современный сетевой трафик с атаками, доступны исходные файлы/CSV.
- [CTU-13 (Stratosphere IPS)](https://www.stratosphereips.org/datasets-ctu13) – 13 сценариев ботнет-трафика, смешанного с нормальным.

Примечание: часто существуют зеркала на Kaggle, но первоисточник предпочтительнее.

### Трек B / текст (спам, фишинг, письма)

- [SMS Spam Collection (UCI)](https://archive.ics.uci.edu/ml/datasets/sms%2Bspam%2Bcollection) – размеченные SMS (spam/ham).
- [Apache SpamAssassin public corpus](https://spamassassin.apache.org/old/publiccorpus/) – архивы писем "spam/ham".
- [Enron Email Dataset (CMU)](https://www.cs.cmu.edu/~enron/) – большой корпус писем (без "готовых" labels под ИБ, но годится для задач классификации/поиска/сетевого анализа общения).

### Трек B / фишинг по URL/признакам (таблично, но "про фишинг")

- [PhiUSIIL Phishing URL Dataset (UCI, 2024)](https://archive.ics.uci.edu/dataset/967/phiusiil%2Bphishing%2Burl%2Bdataset) – крупный набор URL и признаки.
- [Phishing Websites (UCI)](https://archive.ics.uci.edu/ml/datasets/phishing%2Bwebsites) – табличные признаки для классификации фишинговых сайтов.

### Трек C / логи и аномалии

- [anomaly-detection-log-datasets (AIT-AECID)](https://github.com/ait-aecid/anomaly-detection-log-datasets) – набор скриптов и указателей на публичные лог-датасеты (HDFS и др.).
