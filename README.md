# Markdown + LaTeX Studio

Локальный браузерный рендерер для Markdown, LaTeX и ASCII flowchart в одном окне.

## About

### Для GitHub `About` (краткое описание)
`Browser Markdown + LaTeX + Flowchart renderer with instant preview, light/dark themes, and PDF export.`

### Для GitHub `Topics`
`markdown`, `latex`, `mathjax`, `flowchart`, `renderer`, `javascript`, `single-file-app`

## Возможности

- Мгновенный рендер Markdown (`marked`).
- Рендер LaTeX через MathJax (`$...$`, `$$...$$`, `\(...\)`, `\[...\]`, `\begin...\end...`).
- Поддержка ASCII flowchart в блоках ```flowchart.
- Переключение светлой/тёмной темы.
- Сворачивание/разворачивание окна ввода.
- Сворачивание/показ справки.
- Экспорт в PDF через системный диалог печати.
- Сохранение UI-настроек в `localStorage`.

## Быстрый старт

1. Клонируйте репозиторий:

```bash
git clone https://github.com/dwnmf/LATEX_render.git
cd LATEX_render
```

2. Откройте `index.html` в браузере.

Все зависимости подключаются через CDN, отдельная сборка не нужна.

## Синтаксис

### Markdown

```md
## Заголовок

**Жирный текст**, списки, таблицы, блоки кода и т.д.
```

### LaTeX

```tex
Встроенно: $E=mc^2$

Блочно:
$$
\sum_{i=1}^{n} i^2 = \frac{n(n+1)(2n+1)}{6}
$$
```

### Flowchart

````md
```flowchart
st=>start: Старт
op=>operation: Шаг
cond=>condition: Готово?
e=>end: Выход

st->op->cond
cond(yes)->e
cond(no)->op
```
````

## Управление

- `Ctrl + Enter` / `Cmd + Enter` — рендер.
- `Рендер` — ручной рендер.
- `Очистить` — очистка редактора.
- `Экспорт PDF` — печать/сохранение PDF.
- `Свернуть ввод` — скрытие панели ввода и расширение превью.
- `Справка` — показать/скрыть подсказки.
- `Тема` — переключение между светлой и тёмной темой.

## Технически

- Один файл приложения: `index.html`.
- Без фреймворков, чистый HTML/CSS/JS.
- Библиотеки:
  - `marked`
  - `MathJax`
  - `flowchart.js` + `Raphael`

## Ограничения

- Внешние CDN должны быть доступны.
- Рендер зависит от возможностей браузера (рекомендуются актуальные версии Chrome/Edge/Firefox).
- PDF-экспорт использует нативный диалог печати браузера.

## Лицензия

Если нужна отдельная лицензия, добавьте `LICENSE` в репозиторий.
