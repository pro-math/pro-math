# Проект ProMath

## Описание проекта

Проект ProMath – это веб-приложение, созданное в рамках конкурса "Задание для проведения отборочного этапа II Всероссийского хакатона «Обучаюсь. Проектирую. Программирую. Будущее»" в направлении "Программирование". Партнерами этого конкурса являются Тинькофф и Центральный университет. Наш проект "Математический генератор" создан с целью возрождения интереса к математике и помощи пользователям в развитии и проверке своих математических навыков.

## Требования к приложению

- **Состав**: Приложение состоит из серверной и клиентской частей, а также подключено к базе данных.
- **Масштабируемость**: Приложение разработано с учетом возможности масштабирования.
- **Безопасность**: Регистрация и аутентификация пользователей должны быть безопасными.
- **Интерфейс**: Интуитивно понятный и привлекательный интерфейс, оптимизированный для мобильных устройств.
- **Генерация примеров**: Генерация случайных математических примеров с выбором уровня сложности и типа примеров.
- **Решение примеров**: Мгновенная проверка правильности ответа и возможность пропустить пример.

## Особенности платформы

### Backend (API)

- **FastAPI**: Высокопроизводительный фреймворк, обеспечивающий быструю разработку API.
- **Poetry**: Инструмент для управления зависимостями и виртуальными окружениями Python, обеспечивающий чистоту и простоту управления зависимостями.
- **PostgreSQL**: Надежная и масштабируемая реляционная база данных.
- **Alembic**: Инструмент для управления миграциями базы данных, обеспечивающий легкость в поддержке и развертывании изменений схемы.
- **PyJWT**: Библиотека для работы с JSON Web Token (JWT) в Python, обеспечивающая безопасную аутентификацию и авторизацию пользователей.

### Frontend

- **Vue.js**: Прогрессивный JavaScript-фреймворк для создания пользовательских интерфейсов, обеспечивающий быструю и масштабируемую разработку.
- **DaisyUI**: Набор компонентов для Tailwind CSS, делающий разработку пользовательского интерфейса быстрой и удобной.
- **Pinio**: Инструмент для управления состоянием в приложениях Vue.js, обеспечивающий эффективное управление данными.
- **Tailwind CSS**: Современный CSS-фреймворк, позволяющий быстро создавать красивые пользовательские интерфейсы.

### Мобильное приложение

- **Kotlin**: Мощный и выразительный язык программирования для разработки мобильных приложений под платформу Android.
- **Ktor Client**: Клиентское API-фреймворк для Kotlin, обеспечивающий асинхронную обработку HTTP-запросов.
- **Koin**: Легковесный инструмент для управления зависимостями в Kotlin, обеспечивающий чистоту и простоту разработки.
- **Jetpack Compose**: Современный фреймворк для создания пользовательских интерфейсов в приложениях Android, обеспечивающий декларативный подход к созданию интерфейса.
- **Vico**: Библиотека для управления состоянием в мобильных приложениях Kotlin, обеспечивающая эффективное управление данными.
- **Coil**: Библиотека для загрузки изображений в приложениях Android, обеспечивающая быструю и эффективную загрузку и кэширование изображений.

### Docker

Для развертывания проекта используется Docker, что обеспечивает удобство и надежность в управлении окружением разработки и продакшена.

### Аутентификация

Пользователи могут зарегистрироваться и войти в свой аккаунт с помощью уникального имени пользователя и пароля. При аутентификации на сервере генерируется JWT-токен, обеспечивающий безопасную авторизацию.

## Личный кабинет

Пользователи имеют доступ к личному кабинету, где они могут просматривать историю своих игр, отслеживать свой прогресс и результаты, а также изучать свои достижения.

## Прогресс и мотивация

Проект обладает системой мотивации, основанной на наградах и ачивках за выполнение определенных задач. Это мотивирует пользователей активнее использовать приложение и развивать свои математическические навыки.

## Интерфейс

Платформа обладает привлекательным и интуитивно понятным интерфейсом, который адаптирован как для использования на сайте, так и на мобильных устройствах. Пользователи могут выбирать одну из шести тем для персонализации интерфейса, что делает его еще более привлекательным и приятным.

На главном экране ProMath пользователи обнаружат поле для начала игры, где им доступны различные настройки, позволяющие настроить игровой процесс под свои предпочтения и уровень навыков. Вот основные настройки, доступные пользователям:

### Выбор математических операций

Пользователи могут выбирать одну или несколько математических операций, которые они хотят использовать в игре. Доступные операции включают сложение, вычитание, умножение и деление.

### Выбор сложности игры

Пользователи могут выбирать уровень сложности игры, который определяет диапазон чисел, используемых в математических примерах. Доступные уровни сложности включают 10 (примеры с разрядами десятков), 100 (с разрядами сотен) и 1000 (с разрядами тысяч).

### Вариант игры

Пользователи могут выбирать вариант игры: на время или на количество. 

- **Игра на время**: В этом режиме игрокам предоставляется ограниченное время на решение как можно большего количества примеров. Они могут выбрать продолжительность игры из предложенных вариантов: 15, 30, 60 или 90 секунд.

- **Игра на количество**: В этом режиме игрокам предоставляется определенное количество примеров для решения. Они могут выбрать количество примеров из предложенных вариантов: 10, 15, 20 или 30.

Эти настройки позволяют пользователям настроить игровой процесс так, чтобы он соответствовал их уровню навыков, времени и предпочтениям, делая игру более увлекательной и персонализированной.

## Настройки игры

В игре пользователи могут настраивать различные параметры, такие как выбор математических операций (сложение, вычитание, умножение, деление), уровень сложности (10, 100, 1000), и тип игры (на время или на количество). Это позволяет каждому пользователю настроить игровой процесс под свои предпочтения и уровень навыков.

## Отслеживание прогресса

Пользователи могут отслеживать свой прогресс и результаты, сохраняя историю своих игр и просматривая статистику. Графики и диаграммы помогают визуализировать и анализировать свой прогресс в различных аспектах игры.

## Идеальное решение для всех

Проект ProMath идеально подходит для широкого круга пользователей, начиная от учеников и студентов, желающих улучшить свои математические навыки, и заканчивая любителями математики, которые просто хотят развлечься и провести время с пользой. Благодаря своей простоте, удобству и масштабируемости, платформа ProMath станет незаменимым помощником для всех, кто интересуется математикой и желает развивать свои навыки игрой.

## Инструкция по деплою

В каждом отдельном репозитории (backend (https://github.com/pro-math/backend), frontend (https://github.com/pro-math/frontend), mobile (https://github.com/pro-math/mobile-android)) вы найдете подробную инструкцию по развертыванию проекта, что обеспечит простоту и надежность в развертывании приложения на вашем сервере или локальной машине. Для проверки сначала запустите по инструкции backend, затем frontend.

Присоединяйтесь к ProMath и вместе мы будем развивать математические навыки и исследовать прекрасный мир математики!

Скринкасты: https://disk.yandex.ru/d/OcaEswoIYT3t9g

