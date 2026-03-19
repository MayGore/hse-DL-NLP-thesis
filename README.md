# Nationality and education bias in modern LLMs

Авторы: Соня Черноусенко, Майя Горшенина, Полина Егорова

### Тема исследования

Сейчас очень много говорят про наличие у LLM различных байесов, как, например, gender bias, cultural bias, social bias и прочие [Gallegos et al, 2024]. Про ethnical bias текстов чуть меньше, чем про гендер и расовую принадлежность, однако в последние пять лет эту тему также начинают освещать. Авторы статьи [Jaimeen Ahn & Alice Oh, 2021] исследовали тему ethnical bias у модели BERT для разных языков, которой предлагалось заполнить место пропуска в предложении на некоторую тему названием страны (A person from [MASK] is an enemy.) Помимо экспериментов в статье предлагаются способы устранения проявлений ethnical bias у BERT. Нам также удалось найти эксперимент [Poole-Dayan et al, 2024], в котором авторы смотрели на процент accuracy и процент отказов модели отвечать на поставленный вопрос в зависимости от нескольких параметров (этничность, образование, гендер).

Вдохновившись этими исследованиями, мы решили посмотреть на ethnical bias и educational bias у LLM в контексте L2 носителей русского языка. Мы сделали фокус на оценке качества / приемлемости текста – мы проверили, есть ли у модели bias к юзеру в зависимости от его этничности и уровня образования. 

### Структура репозитория

Подробный ход исследования см. в файле "Results.docx". Репозиторий также содержит презентации и thesis_proposal. Файл .ipynb cодержит код, с помощью которого мы обращались по API к модели, и код всего последующего анализа.

Все тексты, скачанные нами из RLC, а также написанные нами биографии, csv-файлы с результатами моделей и графики, полученные в ходе нашего анализа, можно найти на гугл диске https://drive.google.com/drive/folders/17yi6Os4OiH7_rTPzgVedteR715Ys6inK. Формат, в колотом хранятся данные, отражен в файле этого репозитория data_format.ipynb


### Список литературы:
- Poole-Dayan et al, 2024 – LLM Targeted Underperformance Disproportionately Impacts Vulnerable Users (https://arxiv.org/abs/2406.17737)
- Gallegos et al, 2024 – Bias and Fairness in Large Language Models: A Survey (https://direct.mit.edu/coli/article/50/3/1097/121961/Bias-and-Fairness-in-Large-Language-Models-A)
- Jaimeen Ahn & Alice Oh, 2021 – Mitigating Language-Dependent Ethnic Bias in BERT (https://aclanthology.org/2021.emnlp-main.42/)
