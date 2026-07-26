<p align="center">
  <img src="public/icon/icon-128.png" height="128">
  <h1 align="center">7TV Extension — Ban 1s</h1>
</p>

<p align="center">
  A modified version of <a href="https://github.com/SevenTV/Extension">7TV Web Extension</a> with an added 1-second ban button for Twitch chat moderation.
</p>

---

## What's Changed

A new **Ban 1s** button has been added to the chat moderation panel. It sits alongside the existing Ban, Timeout, Warn, and Delete buttons, giving moderators a quick way to issue a 1-second ban.

### Button Layout (left to right):

| Button | Action |
|--------|--------|
| Ban | Permanent ban |
| **Ban 1s** | 1-second ban (new!) |
| Timeout | 10-minute timeout |
| Warn | Warning prompt |
| Delete | Delete message |

> The Ban 1s button is only visible to channel moderators.

---

## Screenshot

<p align="center">
  <img src="Screenshot_4.jpg" width="100%">
</p>

---

## Installation

### Chrome / Brave / Edge

1. Download and extract the [latest release](https://github.com/aoooky/seventv-extension-ban1s/releases) or ZIP archive
2. Open `chrome://extensions`
3. Enable **Developer mode** (toggle in the top right)
4. Click **Load unpacked**
5. Select the `dist` folder from the extracted archive
6. Done! Open Twitch and enjoy the new button

### Firefox

1. Download and extract the release
2. Open `about:debugging#/runtime/this-firefox`
3. Click **Load Temporary Add-on**
4. Select the `manifest.json` file inside the `dist` folder

---

## Building from Source

```bash
git clone https://github.com/aoooky/seventv-extension-ban1s.git
cd seventv-extension-ban1s
npm install
npx cross-env NODE_ENV=production npx vite build --config vite.config.mts
npx cross-env NODE_ENV=production npx vite build --config vite.config.background.mts
npx cross-env NODE_ENV=production npx vite build --config vite.config.content.mts
npx cross-env NODE_ENV=production npx vite build --config vite.config.worker.mts
```

Build output will be in the `dist/` folder.

---

## Based On

- [SevenTV Extension](https://github.com/SevenTV/Extension) — original extension
- License: MIT

---

# [Русский](#русское-описание)

---

## Русское описание

### Что изменено

Добавлена новая кнопка **Ban 1s** в панель модерации чата. Теперь рядом с обычными кнопками Ban, Timeout, Warn и Delete появилась дополнительная кнопка для мгновенного бана на 1 секунду.

### Расположение кнопок (слева направо):

| Кнопка | Действие |
|--------|----------|
| Ban | Перманентный бан |
| **Ban 1s** | Бан на 1 секунду (новая!) |
| Timeout | Таймаут на 10 минут |
| Warn | Предупреждение |
| Delete | Удалить сообщение |

> Кнопка Ban 1s отображается только для модераторов канала.

### Установка

**Chrome / Brave / Edge:**
1. Скачайте и распакуйте релиз или ZIP-архив
2. Откройте `chrome://extensions`
3. Включите **Режим разработчика** (Developer mode)
4. Нажмите **Загрузить распакованное расширение** (Load unpacked)
5. Выберите папку `dist`
6. Готово!

**Firefox:**
1. Скачайте и распакуйте релиз
2. Откройте `about:debugging#/runtime/this-firefox`
3. Нажмите **Загрузить временное дополнение**
4. Выберите файл `manifest.json` в папке `dist`

### Сборка из исходников

```bash
git clone https://github.com/aoooky/seventv-extension-ban1s.git
cd seventv-extension-ban1s
npm install
npx cross-env NODE_ENV=production npx vite build --config vite.config.mts
npx cross-env NODE_ENV=production npx vite build --config vite.config.background.mts
npx cross-env NODE_ENV=production npx vite build --config vite.config.content.mts
npx cross-env NODE_ENV=production npx vite build --config vite.config.worker.mts
```

### Основано на

- [SevenTV Extension](https://github.com/SevenTV/Extension) — оригинальное расширение
- Лицензия: MIT
