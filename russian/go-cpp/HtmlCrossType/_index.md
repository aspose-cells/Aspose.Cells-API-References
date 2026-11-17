---
title: "HtmlCrossType Перечисление"
linktitle: "HtmlCrossType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "HtmlCrossType enum. Инкапсулирует объект, представляющий htmlcrosstype в Go."
type: docs
weight: 200
url: /ru/go-cpp/htmlcrosstype/
---

## HtmlCrossType Enum

Представляет пять типов HTML‑перекрестных строк.

```go

type HtmlCrossType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [Default](./default/) | Отображать как MS Excel,зависит от следующей ячейки.Если следующая ячейка null,строка будет пересекаться,или будет обрезана |
| [MSExport](./msexport/) | Отображать строку как MS Excel при экспорте html. |
| [Cross](./cross/) | Отображать HTML‑строку, эта производительность при создании больших html‑файлов будет более чем в десять раз быстрее, чем установка значения Default или FitToCell. |
| [CrossHideRight](./crosshideright/) | Отображать HTML‑строку и скрывать правую строку, когда тексты перекрываются. |
| [FitToCell](./fittocell/) | Отображать строку только в пределах ширины ячейки. |
