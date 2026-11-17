---
title: "Перечисление MergedCellsShrinkType"
linktitle: "MergedCellsShrinkType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление MergedCellsShrinkType. Инкапсулирует объект, представляющий mergedcellsshrinktype в Go."
type: docs
weight: 200
url: /ru/go-cpp/mergedcellsshrinktype/
---

## MergedCellsShrinkType Enum

Представляет стратегию сжатия объединённых ячеек для операций, таких как удаление пустых строк/столбцов.

```go

type MergedCellsShrinkType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [None](./none/) | Оставляет объединённые ячейки без каких-либо изменений. |
| [ShrinkToFit](./shrinktofit/) | Уменьшает объединённую область при необходимости, удаляя строки снизу или столбцы справа, при этом обеспечивая видимость всего содержимого. |
| [KeepHeaderOnly](./keepheaderonly/) | Сохраняет только строки/столбцы заголовков объединённой области, когда верхняя‑левая ячейка объединённой области не пуста. |
