# Быстрый деплой на Vercel

## Текущий статус

✅ Проект готов к деплою
✅ Все файлы настроены
✅ Vercel CLI установлен локально

## Следующие шаги

### 1. Авторизуйтесь в Vercel

```bash
cd /Users/ttikeev/Desktop/test/5_prototype/country-selector-prototype
npx vercel login
```

Откроется браузер для авторизации. Войдите в аккаунт Vercel.

### 2. Задеплойте проект

```bash
npx vercel
```

Для production деплоя:

```bash
npx vercel --prod
```

## Альтернатива: Деплой через веб-интерфейс

Если CLI не работает, используйте веб-интерфейс:

1. Перейдите на https://vercel.com
2. Нажмите "Add New Project"
3. Загрузите папку `country-selector-prototype` или подключите Git репозиторий
4. Vercel автоматически определит настройки
5. Нажмите "Deploy"

## После деплоя

Вы получите URL вида:
- Preview: `https://country-selector-prototype-xxx.vercel.app`
- Production: `https://country-selector-prototype.vercel.app`
