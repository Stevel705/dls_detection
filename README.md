# Проект для Deep Learning School 
## Тема: Detection 
Описание:

Основная часть: 
- настройка нейросети-детектора

1 сценарий:

- написание веб/мобильного демо 

- встраивание модели в интерфейс 

Общий этап работы:

    1). Выбор фреймворка/библиотеки для использования детектора 

    2). Запуск детектора на случайных изображениях 
1 сценарий:

    3). Выбор фреймворка/библиотеки для разработки веб/мобильного демо 
    4). Разработка демо 
    5). Встраивание модели-детектора в демо 
    6). Тестирование демо 
    7). Оформления демо для показа другим людям 


## Запуск:
    python app.py

    go to: http://127.0.0.1:5000/ 


Для детекции через GET запрос:

    http://127.0.0.1:5000/detect?url=https://example.com/images/test.jpg

    где https://example.com/images/test.jpg - ссылка на изображение 

Чтобы загрузить свое изображение 
    
    http://127.0.0.1:5000/upload

Использование webcam в браузере для детекции в реальном времени. 

    python webcam_streaming.py 
    
    go to: http://127.0.0.1:5000/




#
Пока для инференса используется предобученная сеть из torchvision на датасете COCO.
Где используется 90 классов. 

Примеры работы детектирования:
    Фото с телефона: 
    ![Source](src/img_test.jpg)
    ![Detect](src/img_test_detect.jpg)
    Фото из интернета: 
    ![Source](src/url.jpeg)
    ![Detect](src/url_detect.jpeg)

TODO:

    Сделать связку с Detectron2
    Создать pipeline с обучением из второго сценария и инференсом первого
<!-- 

Сделать второй сценарий:
    
    - предобработка датасета
    - обучение нейросети
    - измерение метрик   -->
