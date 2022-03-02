# Тестовое задание для Фабрики Решений

---

### Описание

---
Проект предназначен для рассылки сообщений клиентам в зависимости от категорий и кода используемого оператора в определенный промежуток времени.
В проекте созданы модели OperatorCode, Tag, Client, MessageList, Message, а также настроена кастомная модель User.

---

### API

Настроен для просмотра, создания и изменения модели Client и MessageList с использованием:
viewsets:
  - ClientViewSet
  - MessageListViewSet и сериализаторов
serialializers:
  - ClientSerializer
  - MessageListCreateViewSet
  - MessageListGetSerializer

По запросу на URL запускается скрипт рассылки актуальных сообщений.

---

### Установка


---

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/camousmen/api_yamdb.git
```

```
cd fabrique
```

Cоздать и активировать виртуальное окружение:

```
python -m venv env
```

```
source venv/Scripts/activate
```

```
python -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python manage.py migrate
```

Запустить проект:

```
python manage.py runserver
```

---


