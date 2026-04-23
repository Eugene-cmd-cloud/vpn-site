# GitHub Pages VPN links hub

Это исправленный вариант сайта: главная страница только показывает прямые ссылки,
а приложениям нужно давать ссылки на конкретные файлы в `subs/`, а не на `/vpn-site/`.

## Что уже внутри

- `subs/v2rayng-moldova-sub.txt` — base64 subscription для клиентов, которые ждут subscription по URL
- `subs/vless-moldova-uri.txt` — обычная VLESS ссылка
- `data/links.json` — список ссылок, который рендерится на главной странице
- `index.html` — сайт

## Прямые ссылки после публикации

Если репозиторий называется `vpn-site`, то будут такие URL:

- Главная страница:
  `https://eugene-cmd-cloud.github.io/vpn-site/`

- Subscription файл:
  `https://eugene-cmd-cloud.github.io/vpn-site/subs/v2rayng-moldova-sub.txt`

- Обычная VLESS ссылка:
  `https://eugene-cmd-cloud.github.io/vpn-site/subs/vless-moldova-uri.txt`

## Как добавить новую ссылку

1. Загрузи новый файл в папку `subs/`
2. Открой `data/links.json`
3. Добавь новый объект в массив `items`

Пример:

```json
{
  "title": "Germany subscription",
  "description": "Base64 subscription для клиента",
  "type": "subscription",
  "path": "subs/v2rayng-germany-sub.txt"
}
```

## Moldova base64 subscription

```text
dmxlc3M6Ly8yZjkxMDdjYi05YWYwLTRjOTQtYTg5ZC01MDQzNzIxOGU1ZmFAYXAyLmRpcmVjdGx5LmNoYXQ6NDQzP2VuY3J5cHRpb249bm9uZSZzZWN1cml0eT10bHMmc25pPWFwMi5kaXJlY3RseS5jaGF0JmZwPWNocm9tZSZhbHBuPWgyJTJDaHR0cCUyRjEuMSZpbnNlY3VyZT0wJmFsbG93SW5zZWN1cmU9MCZ0eXBlPXdzJmhvc3Q9YXAyLmRpcmVjdGx5LmNoYXQmcGF0aD0lMkZtZCUyRjEjJUYwJTlGJTg3JUIyJUYwJTlGJTg3JUE5JTIwTW9sZG92YSUyMC0lMjBDaGlzaW5hdQo=
```
