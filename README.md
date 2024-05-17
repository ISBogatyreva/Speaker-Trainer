# Speaker-Trainer

Мобильное приложение "Тренажер докладчика": подсистема обработки речи и серверная часть 

Серверная часть приложения расположена в директории Server/trainer_project и имеет следующее содержание:
+ trainer_app - директория с кодом приложения (в частности, обработка API запросов - views.py, таблицы базы данных - models.py, обработка файла - file_processing.py)
+ trainer_project - директория с общими настройками файла (в частности - setting.py для подключения к локальной базе данных)
+ manage.py - код для выполнения различных команд Django (запуска сервера, обновления информации о базе данных и т.д.)
+ requirements.txt - библиотеки Python, необходимые для работы

Подсистема обработки речи расположена в Server/trainer_project/trainer_app/speech_processing и имеет следующее содержание:
+ 6 файлов-классов обработки (automatic_speech_recognition, background_noise, emotions, filler_words, intelligibility, speech_rate)
+ 1 файл-общий класс подсистемы, объединяющий вышеуказанные классы (automatic_speech_recognition)
+ директорию tests - тестирование классов
+ файлы расширения .sav - используемые модели

Для корректной работы необходимо разместить директорию с файлами подсистемы обработки речи в Server/trainer_project/trainer_app

Демонстрация работы приложения - https://drive.google.com/file/d/1hUK07LR7muuMa8ucsuX_14XACEoE3KYQ/view?usp=sharing

Демонстрация серверной части (запросы Postman) и административного функционала (графики и CRUD пользователей и файлов) - https://drive.google.com/file/d/1sakZDn3aIhQmJ5ygBBQWxbMcCITNDq6U/view?usp=sharing
