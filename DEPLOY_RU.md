# Инструкция по запуску KREDA Agency на GitHub + Vercel

## 1. Создать новый GitHub репозиторий

1. Открой GitHub.
2. Нажми `New repository`.
3. Назови репозиторий, например:

```text
kreda-agency-website
```

4. Можно сделать Public или Private.
5. Нажми `Create repository`.

## 2. Загрузить файлы

Загрузи в корень репозитория все файлы из этой папки:

```text
index.html
vercel.json
README.md
DEPLOY_RU.md
.gitignore
assets/kreda-logo.svg
```

Важно: `index.html` должен быть именно в корне, не внутри дополнительной папки.

## 3. Создать новый проект в Vercel

1. Открой Vercel.
2. Нажми `Add New` → `Project`.
3. Выбери новый GitHub репозиторий.
4. В настройках проекта укажи:

```text
Framework Preset: Other
Root Directory: ./
Build Command: оставить пустым
Output Directory: ./
Install Command: оставить пустым
```

5. Нажми `Deploy`.

## 4. Если снова будет 404

Проверь:

```text
1. index.html лежит в корне репозитория.
2. Название файла строго index.html, маленькими буквами.
3. В Vercel Root Directory указан ./.
4. Output Directory указан ./.
5. Проект Vercel подключен к правильному GitHub репозиторию.
```

## 5. Проверка локально

В терминале из папки сайта:

```bash
python3 -m http.server 8000
```

Открой:

```text
http://127.0.0.1:8000
```
