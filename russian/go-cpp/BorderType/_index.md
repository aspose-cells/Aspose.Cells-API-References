---
title: "Перечисление BorderType"
linktitle: "BorderType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление BorderType. Инкапсулирует объект, представляющий bordertype в Go."
type: docs
weight: 200
url: /ru/go-cpp/bordertype/
---

## BorderType Enum

Перечисляет типы границ и диагональных линий.

```go

type BorderType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [LeftBorder](./leftborder/) | Представляет левую границу. |
| [RightBorder](./rightborder/) | Представляет правую границу. |
| [TopBorder](./topborder/) | Представляет верхнюю границу. |
| [BottomBorder](./bottomborder/) | Представляет нижнюю границу. |
| [DiagonalDown](./diagonaldown/) | Представляет диагональную линию от верхнего левого к правому нижнему. |
| [DiagonalUp](./diagonalup/) | Представляет диагональную линию от нижнего левого к правому верхнему. |
| [Vertical](./vertical/) | Только для динамического стиля, например условного форматирования, сводных таблиц. |
| [Horizontal](./horizontal/) | Только для динамического стиля, например условного форматирования, сводных таблиц. |
| [SideBorders](./sideborders/) | Указывает четыре боковые границы: <see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/> и <see cref="BottomBorder"/>. |
| [Diagonal](./diagonal/) | Специальное сочетание нескольких границ для удобства пользователя в некоторых API. Указывает диагональные границы <see cref="DiagonalUp"/> и <see cref="DiagonalDown"/>. |
| [DynamicStyleBorders](./dynamicstyleborders/) | Указывает <see cref="Vertical"/> и <see cref="Horizontal"/> динамического стиля. |
| [None](./none/) | Границы не указаны. |
