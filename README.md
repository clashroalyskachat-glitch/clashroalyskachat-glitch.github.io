# НКС — стартовая страница

Корень сайта: выбор между расписанием и библиотекой.

Адрес: **https://clashroalyskachat-glitch.github.io/**

| Раздел | Адрес |
|---|---|
| Расписание | https://clashroalyskachat-glitch.github.io/mypars/ |
| Библиотека | https://clashroalyskachat-glitch.github.io/mypars/library/ |

## Файлы

| Файл | Назначение |
|---|---|
| `index.html` | разметка: шапка, заголовок, две карточки-ссылки, подвал |
| `styles.css` | оформление, тёмная тема, анимации, адаптив |
| `app.js` | переключатель темы, дата, плавный уход со страницы |
| `favicon.svg` | иконка |

## Публикация

Корень `github.io` отдаётся только из репозитория с именем
**`clashroalyskachat-glitch.github.io`** — это особенность GitHub Pages.

```bash
git init
git add .
git commit -m "Стартовая страница"
git branch -M main
git remote add origin https://github.com/clashroalyskachat-glitch/clashroalyskachat-glitch.github.io.git
git push -u origin main
```

Затем в репозитории: **Settings → Pages → Source: Deploy from a branch →
Branch: main / (root)**.

Ссылки в карточках абсолютные (`/mypars/` и `/mypars/library/`), поэтому
страница должна открываться именно с корня домена.

## Локальный просмотр

```bash
python -m http.server 8094
```

Открыть `http://localhost:8094`. Ссылки на разделы при этом не работают —
они ведут на настоящий домен; локально проверяется только внешний вид.
