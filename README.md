# Network cheat sheets

[Русский](#русский) · [English](#english)

---

## Русский

Три автономных HTML-страницы: ручной расчёт сетей, разбиение по префиксам и оформление L2/L3-схем. Без сборки, без зависимостей, без интернета — скачал файл, открыл в браузере. Каждая страница двуязычная, переключатель `RU / EN` в правом верхнем углу.

### Что внутри

| Файл | О чём |
|---|---|
| [`subnets.html`](subnets.html) | Интерактивная шпаргалка по префиксам `/1`–`/32`. Доска: исходная сеть и три уровня деления пополам, клик по блоку — провалиться внутрь. Полная таблица: маска, wildcard, число адресов и хостов, шаг, октет границы. |
| [`guide.html`](guide.html) | Расчёт адреса сети, broadcast и диапазона хостов по префиксу через размер блока, без двоичного вида. Таблица шагов для последнего октета, пять разобранных задач (кому принадлежит адрес, деление на равные части, VLSM, граница в третьем октете, «сколько хостов → какая маска»), калькулятор с пошаговым выводом, типичные ошибки. |
| [`diagrams.html`](diagrams.html) | Разделение документации на L2 и L3: состав каждой схемы, обозначения, офис на 40 человек в двух вариантах (SVG), таблицы VLAN/адресации, карта портов и устройств, правила оформления, порядок работы с нуля, инструменты, типичные ошибки. |

### Как открыть или скачать

- **Посмотреть онлайн** — GitHub Pages:
  [subnets](https://alexandrd7.github.io/network-cheatsheets/subnets.html) ·
  [guide](https://alexandrd7.github.io/network-cheatsheets/guide.html) ·
  [diagrams](https://alexandrd7.github.io/network-cheatsheets/diagrams.html)
- **Скачать всё одним архивом** — [ZIP](https://github.com/AlexandrD7/network-cheatsheets/archive/refs/heads/main.zip)
- **Скачать один файл** — открыть его в таблице выше и нажать **Download raw file**. `Ctrl+S` на странице Pages тоже сохраняет файл целиком: разметка, стили, скрипты и оба языка лежат внутри одного HTML.
- **Через git:**

```bash
git clone https://github.com/AlexandrD7/network-cheatsheets.git
```

Файлы работают офлайн, ничего не грузят со стороны и никуда не отправляют данные. Схемы в `diagrams.html` — inline SVG, так что масштабируются без потери качества и печатаются как есть.

---

## English

[↑ Русский](#русский)

Three standalone HTML pages: subnet math by hand, prefix splitting, and L2/L3 network diagramming. No build step, no dependencies, no internet — download a file and open it in a browser. Every page is bilingual, with an `RU / EN` switch in the top right corner.

### Contents

| File | What it covers |
|---|---|
| [`subnets.html`](subnets.html) | Interactive `/1`–`/32` prefix cheat sheet. A board showing the base network and three levels of halving — click a block to drill into it. Full table: mask, wildcard, address and host counts, block step, boundary octet. |
| [`guide.html`](guide.html) | Deriving the network address, broadcast and host range from a prefix using block size, without binary. The step table for the last octet, five worked tasks (which network an address belongs to, equal splits, VLSM, a boundary in the third octet, host count to mask), a calculator that shows the steps, and common mistakes. |
| [`diagrams.html`](diagrams.html) | Splitting documentation into L2 and L3: what belongs on each, notation, a 40-person office drawn both ways (SVG), VLAN/addressing, port and device tables, layout rules, the order of work from scratch, tools, common mistakes. |

### Viewing and downloading

- **Read online** (GitHub Pages):
  [subnets](https://alexandrd7.github.io/network-cheatsheets/subnets.html?lang=en) ·
  [guide](https://alexandrd7.github.io/network-cheatsheets/guide.html?lang=en) ·
  [diagrams](https://alexandrd7.github.io/network-cheatsheets/diagrams.html?lang=en)
- **Grab everything** — [ZIP archive](https://github.com/AlexandrD7/network-cheatsheets/archive/refs/heads/main.zip)
- **One file** — open it in the table above and hit **Download raw file**, or press `Ctrl+S` on the Pages version. Markup, styles, scripts and both languages live inside the single HTML file.
- **Clone:**

```bash
git clone https://github.com/AlexandrD7/network-cheatsheets.git
```

The pages work offline, load nothing from third parties and send no data anywhere. Diagrams in `diagrams.html` are inline SVG, so they scale without quality loss and print as they are.
