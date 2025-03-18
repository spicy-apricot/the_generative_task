# the_generative_task

Создание генеративных задач на основе фреймворка llmtf (ссылка на фреймворк - https://github.com/RefalMachine/llmtf_open)
![Static Badge](https://img.shields.io/badge/spicy-apricot/the_generative_task)
![GitHub top language](https://img.shields.io/github/languages/top/spicy-apricot/the_generative_task)
![GitHub](https://img.shields.io/github/license/spicy-apricot/the_generative_task)
![GitHub Repo stars](https://img.shields.io/github/stars/spicy-apricot/the_generative_task)
![GitHub issues](https://img.shields.io/github/issues/spicy-apricot/the_generative_task)

Целью этого проекта является обучение меня и тех, кто это посмотрит, в создании генеративных задач. Фреймворк был выбран llmtf в связи с его удобством в подключении языковых моделей с HuggingFace и оценкой ответов.

Были выбраны две генеративные задачи на реализацию: ответы на вопросы по предоставленному тексту и извелечение именованных сущеностей (т.н. NER-задача). 

Чтобы добавить свою генеративную задачу, нужно: 
1) Выбрать генеративную задачу и датасет, по которой модель будет решать генеративную задачу (датасеты брать с https://huggingface.co)
2) Написать класс задачи, как это описано во фрейморке llmtf (https://github.com/RefalMachine/llmtf_open/blob/main/examples/create_new_task.ipynb). Обратите внимание, что имя датасета должно быть взято с HuggingFace, нужно точное название.
3) Подключить модель (опять таки, пример подключения модели с помощью llmtf есть в репозитории llmtf_open). Точное название модели надо также брать с HuggingFace, иначе не будет подключаться.
