# Сплетни Кавалы

Блог на Hugo с темой Bear Blog. Хостинг на GitHub Pages.

## Локальная разработка

```bash
cd blog
hugo server -D
```

Открой http://localhost:1313 в браузере.

## Как написать пост

1. Создай файл:

```bash
hugo new content blog/my-post.md
```

2. Открой `content/blog/my-post.md`, отредактируй:

```markdown
---
title: "Заголовок поста"
date: 2026-07-24
---

Текст поста в формате Markdown.
```

3. Убери `draft: true` если хочешь опубликовать сразу.

## Как опубликовать

```bash
git add -A
git commit -m "New post: my-post"
git push
```

Сайт обновится автоматически через 30-60 секунд.

## Структура

```
content/
  _index.md        — главная страница
  about.md         — страница "О блоге"
  blog/
    my-post.md     — посты
```
