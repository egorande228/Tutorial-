# Tutorial: рабочий процесс по лендингу 1XBET

## Что это за репозиторий
`Tutorial-` хранит только инструкцию/обучение по процессу.

Код сайта находится в отдельном репозитории:
- `https://github.com/egorande228/website-mob-cash-lama`

## Single Source of Truth
Все правки сайта делаются только в:
- локальном клоне `website-mob-cash-lama`
- ветке `main`
- с обязательным `push` после завершенной задачи

`Tutorial-` не используется для редактирования HTML/CSS/JS лендинга.

## Текущая структура сайта (актуально)
Репозиторий сайта: `website-mob-cash-lama`

Ключевые файлы:
- `company-site/index.html`
- `company-site/agent.html`
- `company-site/partner.html`
- `company-site/css/styles.css`
- `company-site/js/main.js`
- `company-site/assets/*`

## Как работать правильно
1. Открыть репозиторий сайта:
   - `cd "/Users/egorande/Documents/New project"`
2. Проверить состояние:
   - `git status -sb`
   - `git remote -v`
3. Внести изменения только в `company-site/*`
4. Проверить локально через HTTP-сервер
5. Зафиксировать и отправить:
   - `git add ...`
   - `git commit -m "..."`
   - `git push origin main`

## Локальный предпросмотр
```bash
cd "/Users/egorande/Documents/New project/company-site"
python3 -m http.server 4173
```
Открыть в браузере:
- `http://127.0.0.1:4173/index.html`

## Публикация / демонстрация
Для временного показа можно использовать Vercel/другой хостинг,
но рабочий источник кода остается `website-mob-cash-lama`.

## Что уже внедрено в сайте (кратко)
- ES/PT/EN переключатель языка в верхнем меню
- Обновленная комиссия `8%` + калькулятор по `8%`
- Обновленные CTA-блоки Telegram/WhatsApp
- Улучшенный блок роста на странице Partner
- Удален блок `Agent Academy`

## Чеклист перед новым чатом
- Проверить синхронизацию: `git fetch origin && git status -sb`
- Убедиться, что `main...origin/main` без отставания
- Продолжать с последнего коммита в `website-mob-cash-lama`
