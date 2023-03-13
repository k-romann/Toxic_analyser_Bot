
# Toxic_analyser_bot: 

Телеграмм бот, созданный для решения задачи бинарной классификации: определить, является ли (и насколько) пользовательское сообщение токсичным в отношении собеседника. 

## Как запустить данный проект:

**Для правильной работы бота необходимо создать виртуальное окружение с использованием requirements.txt**, далее:

```
git clone https://github.com/kostiks/toxic_analyse_telegram_bot
cd https://github.com/kostiks/toxic_analyse_telegram_bot
python -m venv .venv
pip install -r requirements.txt
python bot.py
```

## Этапы подготовки текста и обучения модели:

- 1.Предобработка текста (удаление: знаков препинания, стоп-слов и пр.) 
- 2.Построение векторного представления текста с помощью TfIDF
- 3.Обучение модели бинарной классификации(LogReg)
- 4.Тестирование и релиз бота

### Папка 'models'
- __mod_vectorizer.pkl__  – файл с векторизатором (TfIDF)
- __model.pkl__  – файл с обученной моделью(LogReg)

### Папка 'models'
- __modelling.ipynb__ – файл с процессом обучения моделей и сравнения их качества
- __preprocessing.ipynb__ – файл с процессом предобработки датасета (очистка от знаков препинания, стемминг/лемматизиация и прочее)

