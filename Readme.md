## Установка UI

Установка зависимостей:

```bash
npm i
```

Запуск UI:

```bash
npm start
```

## Установка и настройка окружения

Убедиться, что установлен pip:

```bash
python -m ensurepip --upgrade
```

Установить virtualenv:

```bash
pip install virtualenv
```

Создать виртуальное окружение:

```bash
python -m venv rasa_env
```

Активировать виртуальное окружение:

```bash
source rasa_env/Scripts/activate
```

## Установка Rasa

Установить Rasa через pip:

```bash
pip install rasa
```

При возникновении ошибок:

```bash
pip install setuptools==65.5.1 "wheel<0.40.0"
```

Установить библиотеку Transformers для работы с предобученными LLM моделями, такими как BERT, GPT:

```bash
pip install transformers
```

Проверка версии:

```bash
rasa --version
```

```
Rasa Version      :         3.6.20
Minimum Compatible Version: 3.5.0
Rasa SDK Version  :         3.6.2
Python Version    :         3.10.11
```

## Запуск обучения

Тренируем модель:

```bash
rasa train
```

Запускаем ассистента:

```bash
rasa run --debug --cors "*" --enable-api --log-file log.txt
```
