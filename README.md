# Telegram Sticker & Animated Emoji Collection

Большая коллекция стикерпаков и анимированных эмодзи из Telegram, скачанных и конвертированных в GIF.

## Статистика

| Параметр | Значение |
|---|---|
| Стикерпаков | **1 080** |
| Файлов | **54 955** |
| Общий размер | **7.12 GB** |
| Описание паков | `all.tunel.txt` (6 493 строки) |

### Форматы файлов

| Формат | Количество | Описание |
|---|---|---|
| `.gif` | 25 590 | Анимированные GIF (основной формат) |
| `.webp` | 21 421 | Статичные стикеры WebP |
| `.tgs` | 4 592 | Telegram Lottie анимации |
| `.webm` | 3 318 | Видео стикеры |

## Структура каталога

```
├── AnimatedEmojies/          # Официальные анимированные эмодзи Telegram
├── EmojiAnimations/          # Анимированные эмодзи
├── KomandaDimaMaslennikov/   # Стикерпаки various
├── JujutsuKaisen2/           # Аниме стикеры
├── BrawlStarsEmotes/         # Игровые стикеры
├── CarBrandsSticker/         # Автобренды
├── ...                       # 1 000+ других паков
│
├── all.tunel.txt             # Полный каталог с описанием каждого пака
├── gif.txt                   # Список всех .gif файлов
├── webp.txt                  # Список всех .webp файлов
├── webm.txt                  # Список всех .webm файлов
├── tgs.txt                   # Список всех .tgs файлов
│
├── gif URLs.txt              # URL-ссылки на .gif файлы
├── webp URLs.txt             # URL-ссылки на .webp файлы
├── webm URLs.txt             # URL-ссылки на .webm файлы
└── tgs URLs.txt              # URL-ссылки на .tgs файлы
```

## Категории стикерпаков

- **Аниме** — Jujutsu Kaisen, Attack on Titan, Naruto, Pokemon, Vinland Saga, Demon Slayer
- **Игры** — Brawl Stars, Clash Royale, Fortnite, Minecraft, GTA, Valorant, CS2
- **Бренды** — Nike, Adidas, Apple, Samsung, Google, Tesla, SpaceX
- **Мультфильмы** — Family Guy, Adventure Time, SpongeBob, Rick and Morty
- **Животные** — Коты, собаки, бобры, панды, драконы
- **Мемы** — Pepe, Doge, Troll Face, Rage Comics
- **ТВ-шоу** — Breaking Bad, Game of Thrones, Stranger Things, The Office
- **Кино** — Marvel, DC, Star Wars, Disney, Pixar
- **Эмодзи** — Официальные анимированные эмодзи Telegram

## Файлы со списками

### Полный каталог

- `all.tunel.txt` — подробное описание каждого пака (имя, кол-во стикеров, размер, форматы, подпапки)

### Локальные пути

- `gif.txt` — все пути к GIF файлам
- `webp.txt` — все пути к WebP файлам
- `webm.txt` — все пути к WebM файлам
- `tgs.txt` — все пути к TGS файлам

### URL-ссылки (для прямого доступа)

- `gif URLs.txt` — `https://emoji.darkheavens.ru/...`
- `webp URLs.txt`
- `webm URLs.txt`
- `tgs URLs.txt`

## Использование

### Скачать все GIF

```bash
# Используя gif.txt
while read -r file; do
  mkdir -p "$(dirname "$file")"
  curl -o "$file" "https://emoji.darkheavens.ru/$file"
done < gif.txt
```

### Конвертация TGS в GIF

```bash
pip install tstickers
tstickers -t YOUR_BOT_TOKEN -p STICKER_PACK_NAME --fmt gif --fps 30
```

## Инструменты

- [tstickers](https://github.com/nicegoodboy/tstickers) — CLI для скачивания стикерпаков
- [rlottie-python](https://github.com/nicegoodboy/rlottie-python) — конвертация Lottie в кадры
- [Telethon](https://github.com/LonamiWebs/Telethon) — Telegram API

## Лицензия

Данный проект предназначен для образовательных целей. Все стикеры принадлежат их авторам.
