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

2. Отредактируй `content/blog/my-post.md`:

```markdown
+++
title = "Заголовок поста"
date = 2026-07-24
slug = "my-post"
tags = []
+++

Текст поста в формате Markdown.
```

> Если название кириллическое — обязательно добавляй `slug = "english-name"`, иначе URL будет в процентах.

3. Картинки клади в `static/images/` и подключай так:

```markdown
![Подпись](/images/photo.jpg)
```

## Как опубликовать

```bash
git add -A && git commit -m "edit" && git push
```

Сайт обновится автоматически через 30-60 секунд.

## Структура

```
content/
  _index.md        — главная страница
  about.md         — страница "О блоге"
  blog/
    my-post.md     — посты
static/
  images/          — картинки
```
