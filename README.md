# Image Comparer

Desktop app for comparing two images in `Slide` and `Side-by-side` modes.

## Русский

### Что это?

**Image Comparer** — десктопное приложение для быстрого и удобного сравнения двух изображений.

Поддерживает:

- режим `Slide` с вертикальным разделителем
- режим `Side-by-side` с независимым управлением левой и правой стороной
- загрузку изображений разными способами
- масштабирование, перемещение, миникарту и экспорт текущего вида
- светлую и тёмную темы

### Запуск

1. Откройте `ImageComparer.exe`.

### Основные возможности

- Сравнение двух изображений с вертикальным разделителем в режиме `Slide`
- Режим `Side-by-side` для просмотра изображений в двух независимых половинах окна
- Экспорт текущей видимой области сравнения в `PNG`
- `Mini-map` при сильном увеличении
- Нижняя карусель `Recents` с недавно загруженными изображениями
- Переключение между `Day theme` и `Night theme`
- Режим `Hide UI` для чистого просмотра без интерфейса

### Режимы сравнения

#### Slide

Оба изображения накладываются друг на друга, а вертикальный разделитель показывает границу между ними.

#### Side-by-side

Одно изображение показывается слева, второе справа. Каждую сторону можно масштабировать и перемещать отдельно.

### Natural Aspect Mode

Если пропорции двух изображений сильно различаются, приложение автоматически включает `natural aspect mode`.

В этом режиме:

- изображения не деформируются
- пропорции сохраняются
- показывается временная верхняя плашка с сообщением  
  `Aspect ratios differ significantly, using natural aspect mode.`
- то же сообщение остаётся в статусной строке

Порог срабатывания: примерно `1.35x` по разнице пропорций.

### Способы загрузки изображений

- Кнопки `Load A` и `Load B`
- Клик по стартовым зонам `A` и `B`, когда приложение пустое
- `Drag-and-drop` файлов из Проводника в левую или правую половину окна
- `Drag-and-drop` изображений из карусели `Recents`
- Вставка из буфера обмена через `Ctrl+V`

### Управление

#### В режиме Slide

- Левый клик: установит разделитель под курсор откуда можно сразу начать его перемещать
- Правая кнопка мыши: перемещение текущего вида
- Колесо мыши: увеличение и уменьшение

#### В режиме Side-by-side

- Колесо мыши: масштабирует только ту сторону, над которой находится курсор
- Правая кнопка мыши: перемещает только ту сторону, над которой находится курсор

#### Общие кнопки

- `Swap` — поменять изображения местами
- `Clear` — очистить обе стороны и вернуть стартовые зоны
- `Reset View` — сбросить масштаб и смещение
- `Show Recents` / `Hide Recents` — показать или скрыть нижнюю карусель
- `Hide UI` — скрыть интерфейс и оставить только область изображений
- `Export PNG` — сохранить текущую область сравнения

### Mini-map

Mini-map работает только в режиме `Slide`.

- Появляется при увеличении больше `300%`
- Исчезает при уменьшении до `200%` и ниже
- Красная рамка показывает текущую видимую область
- Можно зажать левую кнопку мыши на mini-map и быстро перемещаться по изображению без изменения масштаба

### Recents

`Recents` по умолчанию скрыт и открывается кнопкой `Show Recents`.

Возможности:

- хранит недавно загруженные изображения
- не дублирует изображения с одинаковым именем файла
- поддерживает прокрутку стрелками
- поддерживает прокрутку нижним слайдером
- поддерживает прокрутку колесом мыши при наведении на карусель
- позволяет перетаскивать изображения обратно в рабочую область

### Export PNG

`Export PNG` работает только в режиме `Slide` и только если загружены оба изображения.

Экспортирует:

- только видимую область сравнения
- изображения и divider
- без остальных элементов интерфейса

После нажатия открывается окно выбора места сохранения.

### Темы

Кнопка `Day theme` / `Night theme` переключает светлую и тёмную темы интерфейса.

### Hide UI

`Hide UI` скрывает:

- верхнюю панель
- подписи изображений
- подсказки
- нижний `Recents`

На экране остаётся только область сравнения и маленькая кнопка `Show UI` для возврата интерфейса.

### Горячие клавиши

- `Ctrl+V` — вставить изображение из буфера обмена
- `F11` — скрыть или вернуть интерфейс

### Нижняя информационная строка

- В обычном режиме показывает статус сравнения и масштаб
- В `Side-by-side` рядом с разрешением каждого изображения также показывается текущий масштаб в процентах

### Как делиться приложением

Если вы отправляете приложение другому человеку:

- делитесь всей папкой приложения, а не только `ImageComparer.exe`
- не отделяйте `assets` от приложения

---

## English

### What it is

**Image Comparer** is a desktop app for quick and convenient comparison of two images.

It supports:

- `Slide` mode with a vertical divider
- `Side-by-side` mode with independent left and right controls
- multiple image loading methods
- zoom, pan, mini-map, and visible-area export
- light and dark themes

### Launch

1. Open `ImageComparer.exe`.
2. Keep the `assets` folder next to the application.

### Core Features

- Two-image comparison with a vertical divider in `Slide` mode
- `Side-by-side` mode for viewing images in two independent halves
- `PNG` export of the current visible comparison area
- `Mini-map` at high zoom levels
- Bottom `Recents` carousel with recently loaded images
- `Day theme` and `Night theme`
- `Hide UI` mode for a clean viewing experience

### Comparison Modes

#### Slide

Both images are layered on top of each other, and the vertical divider defines the boundary between them.

#### Side-by-side

One image is shown on the left, the other on the right. Each side can be zoomed and panned independently.

### Natural Aspect Mode

If the aspect ratios of the two images differ too much, the app automatically switches to `natural aspect mode`.

In this mode:

- images are not deformed
- original proportions are preserved
- a temporary top notification pill appears with the message  
  `Aspect ratios differ significantly, using natural aspect mode.`
- the same message remains in the status line

Trigger threshold: about `1.35x` aspect ratio difference.

### Image Loading Methods

- `Load A` and `Load B` buttons
- Click the `A` and `B` start zones when the app is empty
- `Drag-and-drop` files from Explorer into the left or right half of the window
- `Drag-and-drop` images from the `Recents` carousel
- Paste from clipboard with `Ctrl+V`

### Controls

#### In Slide Mode

- Left click: place the divider under the cursor and drag immediately
- Right mouse button: pan the current view
- Mouse wheel: zoom in and out

#### In Side-by-side Mode

- Mouse wheel: zoom only the side under the cursor
- Right mouse button: pan the left or right image independently
- A center line visually separates both sides and prevents overlap

#### Common Buttons

- `Swap` — swap the two images
- `Clear` — clear both sides and return to the start zones
- `Reset View` — reset zoom and pan
- `Show Recents` / `Hide Recents` — show or hide the bottom carousel
- `Hide UI` — hide the interface and leave only the image area
- `Export PNG` — save the current comparison area

### Mini-map

Mini-map works only in `Slide` mode.

- Appears above `300%` zoom
- Hides again at `200%` zoom and below
- A red rectangle shows the current visible area
- You can drag inside the mini-map with the left mouse button to move the view without changing zoom

### Recents

`Recents` is hidden by default and opens with `Show Recents`.

Features:

- stores recently loaded images
- avoids duplicate entries with the same file name
- supports arrow-based scrolling
- supports bottom scrubber-slider scrolling
- supports mouse wheel scrolling when hovering over the carousel
- allows dragging images back into the working area

### Export PNG

`Export PNG` works only in `Slide` mode and only when both images are loaded.

It exports:

- only the visible comparison area
- images and divider
- without the rest of the interface

After clicking it, the app opens a save dialog.

### Themes

The `Day theme` / `Night theme` button switches between light and dark interface themes.

### Hide UI

`Hide UI` hides:

- the top panel
- image labels
- helper hints
- the bottom `Recents`

Only the comparison area and a small `Show UI` button remain visible.

### Hotkeys

- `Ctrl+V` — paste an image from the clipboard
- `F11` — hide or restore the interface

### Bottom Status Line

- In normal mode it shows comparison status and zoom
- In `Side-by-side`, each image also shows its current zoom percentage next to its resolution

### How to Share the App

If you want to share the app with someone else:

- send the whole application folder, not just `ImageComparer.exe`
- keep the `assets` folder next to the executable
