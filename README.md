# MLOps project geoup 13
![Logotype](./data/a56d354a-4d89-42dc-ada7-09097251ed4d.webp)
### Структура проекта

```
.
├── ...
├── src                              # каталог с исполняемыми скриптами приложения
│   ├── api_app_titanic.py           # API приложение на FASTAPImodels
│   ├── dataset_titanic_modifed.py   # создание "плохого" датасета
│   ├── make_dataset_titanic.py      # сохранение датасета Titanic
│   └── model_titanic.py             # обучение модели на данных датасета Titanic
├── tests                            # unit tests
│   ├── api_app_test.py              # модульное тестирование API приложения
└── └── dataset_test.py              # функциональное тестирование предсказательной способности модели
./doker_container_run.bat            # запуск docker контейнера с приложением из образа (Windows)
./doker_container_run.sh             # запуск docker контейнера с приложением из образа (Unix)
./Dokerfile                          # файл для создания doker образа приложения
./Jenkinsfile                        # конвейер для автоматического развертывания приложения, 
                                       тестирования и сборки doker образа
./predict_titanic.bat                # командный файл для проверки работы API приложения (Windows)
./predict_titanic.sh                 # командный файл для проверки работы API приложения (Unix)
```

> [!NOTE]
Приложение собирается в docker контейнере. Сборка приложения, тестирование и создание docker образа происходит в
автоматическом режиме в `Jenkins` на основе файла сценария `Jenkinsfile`.

> [!IMPORTANT]
После создания docker образа приложения запускается командный файл `doker_container_run.bat (doker_container_run.sh)` для 
сборки и запуска docker контейнера с приложением. Приложение запускается на порту `8091`.

> [!TIP]
Для проверки работы предложения запускаются командные файлы: `predict_titanic.bat (predict_titanic.sh)`

## Команда

```
Аналитик данных – Ластин Максим
Инженер по машинному обучению - Красильников Михаил
Full Stack-разработчик – Казанцев Александр
Тестировщик – Граб Яков
Документалист/технический писатель – Кузнецов Иван

```

## Лицензия

_Python Software Foundation License_
