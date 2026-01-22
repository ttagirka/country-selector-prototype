# Инструкция по деплою на Vercel

## Вариант 1: Деплой через веб-интерфейс Vercel (рекомендуется)

1. Перейдите на [vercel.com](https://vercel.com) и войдите в аккаунт
2. Нажмите "Add New Project"
3. Импортируйте проект из Git репозитория или загрузите папку проекта
4. Vercel автоматически определит настройки для Vite проекта
5. Нажмите "Deploy"

## Вариант 2: Деплой через CLI

### Шаг 1: Исправьте права доступа к npm cache

```bash
sudo chown -R $(whoami) /Users/ttikeev/.npm
```

### Шаг 2: Авторизуйтесь в Vercel

```bash
cd /Users/ttikeev/Desktop/test/5_prototype/country-selector-prototype
npx vercel login
```

Следуйте инструкциям для входа в аккаунт Vercel.

### Шаг 3: Запустите деплой

```bash
npx vercel
```

При первом запуске:
- Vercel спросит настройки проекта (можно использовать значения по умолчанию)
- Vercel автоматически определит настройки для Vite
- Проект будет задеплоен на preview URL

### Шаг 4: Production деплой

```bash
npx vercel --prod
```

или используйте установленный локально vercel:

```bash
npm run deploy
```

## Настройки проекта

Проект уже настроен для Vercel:
- ✅ `vercel.json` - конфигурация для Vercel
- ✅ `package.json` - команды сборки
- ✅ `.gitignore` - исключает ненужные файлы

## После деплоя

После успешного деплоя вы получите:
- Production URL (например: `https://country-selector-prototype.vercel.app`)
- Preview URL для каждого коммита
- Автоматический деплой при пуше в Git (если подключен репозиторий)
