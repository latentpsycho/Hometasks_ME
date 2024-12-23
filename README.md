# Микросервис для хранения и обновления информации о собаках в ветеринарной клинике

# Описание
Микросервис реализует REST API для хранения данных о собаках в ветеринарной клинике и выполнение CRUD-операций (создание,  чтение, обновление и удаление). Также микросервисом предусмотрена фильтрация породы собак по ключевому коду (pk

# Технологии
FastAPI
Uvicorn
Pydantic

# Установка и запуск

1. Создание web-service через render.com
2. Ссылка на действующий репозиторий: latentpsycho/Hometasks_ME
3. Добавление файла requirements.txt в действующий репозиторий latentpsycho/Hometasks_ME
4. Настройка параметров порта:

    ```uvicorn main:app --host 0.0.0.0 --port 10000```
6. После успешного запуска откройте окно браузера и перейдите по адресу: (https://hometasks-me.onrender.com/docs) для ознакомления с микросервисом

# Примеры запросов
1. Получение списка собак GET/dog
```
[
  {
    "name": "Snoopy",
    "pk": 2,
    "kind": "dalmatian"
  },
  {
    "name": "Rex",
    "pk": 3,
    "kind": "dalmatian"
  },
  {
    "name": "Pongo",
    "pk": 4,
    "kind": "dalmatian"
  }
]
```

2. Создание новой собаки POST/dog
```
{
  "name": "Richard",
  "pk": 8,
  "kind": "terrier"
}
```
3. Поиск данных собаки по номеру GET /dog/{pk}

![image](https://github.com/user-attachments/assets/de654e22-f10b-4a96-a4a2-7bae9de4b04f)


4. Обновление данных собаки PATCH /dog/{pk}

```
{
  "name": "Richard",
  "pk": 8,
  "kind": "dalmatian"
}
```

# Результаты работы
Ссылка на готовый веб сервер:
(https://hometasks-me.onrender.com/docs#/default/get_dog_by_pk_dog__pk__get)



 
