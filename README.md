# pabd_cv
Predictive analytics practice repo for computer vision students

## План семинаров

1. Основы работы с bash. 
Система версионирования Git.
Модель разработки GitHub Flow. 
Настройка виртуальной среды python. 
Установка зависимостей, пакетные менеджеры. 
Продвинутые возможности языка python.  

**Результат:** fork репозитория, создание файла services/server_xxx.py.  
Синхронизацию с основным репозиторием labintsev/pabd_cv делать не нужно.
Ваша ветка main должна быть заблокирована от прямых изменения. 
Все изменения вносите в свой репозиторий в ветку main через pull request. 

2. Структура ML проекта, шаблонизация cookiecutter ds. 
Требования к коду: codestyle, linters, formatters, function docs. 
Реализация минимального функционала классификации изображений. 
Тестирование с помощью unittest. 

**Результат:**  Ваш репозиторий должен содержать реализацию сервиса classify с помощью предбученной модели.
Модель должна предсказывать три **наиболее** вероятных класса ImageNet.
Тест должен проверять вхождение класса "Пембрук" в результат предсказания при запущенном сервисе.  


3. Работа с данными и обучение модели. 
Версионирование данных с DVC.  

**Результат:** 
В проекте подключен dvc, в ветке main  . 

4. CLI python. 
[Обучение модели.](https://keras.io/examples/vision/image_classification_from_scratch/)
[Данные](https://drive.google.com/file/d/1PW9uFmww8G9-BwVFwnTitdTFCusx4OuU/view?usp=sharing)

**Результат:** 
Реализация скрипта train.py для обучения модели.  
Результат обучения (модель) сохраняется локально.  
Скрипт предсказания использует обученную модель для бинарной классификации.

5. Валидация модели. 
Добавление новых данных. 
Мониторинг метрик и производительности модели.  

**Результат:** скрипт валидации модели validate.py, деплой модели на препродакшн сервер.   
