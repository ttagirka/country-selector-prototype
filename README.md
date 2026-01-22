# Country Selector Prototype

Прототип экрана выбора кода страны на основе дизайна из Figma.

## Описание

Мобильный интерфейс для выбора кода страны с:
- Статус-баром (мок)
- Кнопкой закрытия (X) в левом верхнем углу
- Заголовком "Choose your country code"
- Поисковой строкой с фильтрацией
- Списком стран с флагами, названиями и телефонными кодами
- Кнопкой "Back" внизу экрана

## Установка и запуск

```bash
# Установить зависимости
npm install

# Запустить dev-сервер
npm run dev

# Собрать для production
npm run build

# Предпросмотр production сборки
npm run preview
```

## Структура проекта

```
country-selector-prototype/
├── src/
│   ├── App.tsx          # Основной компонент прототипа
│   ├── main.tsx         # Точка входа
│   └── styles.css       # Стили и дизайн-токены
├── index.html
├── package.json
├── tsconfig.json
└── vite.config.ts
```

## Особенности

- ✅ Полностью соответствует дизайну из Figma
- ✅ Использует дизайн-токены Exness
- ✅ Адаптивный дизайн для мобильных устройств
- ✅ Поиск по названию страны или телефонному коду
- ✅ Флаги стран загружаются с CDN
- ✅ Интерактивные элементы с hover-эффектами

## Figma ссылка

[Figma Design](https://www.figma.com/design/b0L8ciekQFFzUxOpQ7FWT1/%F0%9F%9A%80-Remove-country-selection-and-change-registration-flow---TFB-807?node-id=5521-77734)
