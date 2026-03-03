# Лабораторная работа №10-11. Создание приложения «Список студентов» с использованием Material Design
Цель работы: Научиться применять принципы Material Design в Androidприложениях с использованием Jetpack Compose. В результате лабораторной работы
будет создано приложение «Список студентов», которое демонстрирует использование
цветовых схем, типографики, форм и анимаций Material Design.

- Поспать
- Поесть
- [x] Выполнить лабу по Android St

## Что мы изучали?

- Добавили изображения студентов в папку `res/drawable/`.
- Создание файла `dimens.xml`. Использовали для хранения размерных значений.
- Настроили `strings.xml`. В нем мы добавили описание для каждой карточки студента.
- Создали в пакете `data` `Data class`, в котором хранили данные.
- Создали `DataSource.kt`, сдесь мы содержали список всех студентов.
- ...
- Добавили цветовую схему с помощью `Material Theme Builder`.
- Поработали с темной и светлой темой телефона.


## Функциональность
- Просмотр списка студентов: Отображает карточки с аватаром, именем, возрастом.
- Расширение карточек: Клик по карточке раскрывает детали.
- App Bar: Заголовок "Студент Лист", иконка профиля, смена темы (light/dark).
- Свайп/навигация: Стрелка назад, меню в расширенном состоянии.
- Темная тема: Автоматическое переключение (аватар, текст адаптированы).

## Технологии

### Основные технологии

- Jetpack Compose — UI toolkit (declarative UI, `@Composable` функции, `Preview`)
- Material Design 3 — дизайн-система (`Card`, `Button`, `dynamic color scheme`)
- MaterialTheme — темы Material 3 (`colorScheme.primary`, `typography`, `shapes`)
- Custom Typography — Abril Fatface + Montserrat шрифты из res/font

### Compose компоненты

`
Card, CardDefaults.cardColors
Button, ButtonDefaults.buttonColors  
Spacer, Column, Row
Text, Icon
LazyColumn (список студентов)
TopAppBar (статус-бар "Студент Лист")
`

### State Management

- `mutableStateOf()` + `by delegate` — реактивное состояние
- `remember { }` — сохранение состояния при recomposition
- `State<T>.value`/`getValue()` — property delegates

### Темизация

- Dynamic Color — светлая/тёмная темы (автопереключение)
- `MaterialTheme.colorScheme` — primary, primaryContainer, surface, onSurface
- Custom `Typography` с FontFamily (R.font.montserrat_regular/bold)

### Ресурсы

- Шрифты: `res/font/abril_fatface_regular.ttf`, `montserrat_regular.ttf`, `montserrat_bold.ttf`
- Изображения: аватары студентов (drawable ресурсы)
- Иконки: Material Icons (стрелки, профиль)

## *Абдулин Ринат Рушанович ИСП-233*