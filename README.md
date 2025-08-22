# Weather App

Это десктопное приложение на **Python (PyQt5)** для отображения текущей погоды в любом городе мира.  
Приложение использует **OpenWeatherMap API** и выводит температуру, описание и эмодзи, соответствующее погоде.

### Приложение обрабатывает:

- Некорректный ввод (неизвестный город)
- Проблемы с интернет-соединением
- Ошибки на стороне API (5xx)


## Функционал
- Ввод названия города
- Получение данных о погоде через OpenWeatherMap API
- Отображение:
  - температуры (в °C)
  - погодного описания (например, *clear sky*, *light rain*)
  - эмодзи соответствующее погоде
- Обработка ошибок (например, если город не найден или нет интернета)

## Структура проекта
```
.
│
├── weather_app.py                    # .py file с кодом приложения
├── requirements.txt                  # .txt file с зависимостями            
└── README.md                       
```



## Основные технологии

- **Python 3.10+**
- **PyQt5** — библиотека для графического интерфейса
- **requests** — библиотека для работы с API
- **OpenWeatherMap API** — источник данных о погоде



## Установка и запуск
1. Клонировать репозиторий:
   ```bash
   git clone https://github.com/your-username/weather-api-app.git
   cd weather-api-app
   ```

2. Установить зависимости::
   ```bash
   pip install -r requirements.txt
   ```

3. Получить бесплатный API-ключ на [OpenWeatherMap](https://openweathermap.org/api)
4. Вставить API-ключ в код (в методе get_weather заменить строку):
    ```bash
   api_key = "YOUR_API_KEY"
   ```
5. Запустить приложение:
    ```bash
   python weather_app.py
   ```
## Интерфейс

![Weather App Screenshot](images/working.png)
![Weather App Screenshot](images/handling_input_error.png)

## Идеи для улучшения:

- Красивые иконки погоды вместо эмодзи
- Тёмная тема интерфейса 
