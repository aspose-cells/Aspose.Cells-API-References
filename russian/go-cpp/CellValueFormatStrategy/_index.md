---
title: "Перечисление CellValueFormatStrategy"
linktitle: "CellValueFormatStrategy"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление CellValueFormatStrategy. Инкапсулирует объект, представляющий cellvalueformatstrategy в Go."
type: docs
weight: 200
url: /ru/go-cpp/cellvalueformatstrategy/
---

## CellValueFormatStrategy Enum

Указывает, как применять стиль к значению ячейки.

```go

type CellValueFormatStrategy int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [None](./none/) | Не отформатировано. |
| [CellStyle](./cellstyle/) | Отформатировано только оригинальным стилем ячейки. |
| [DisplayStyle](./displaystyle/) | Отформатировано отображаемым стилем ячейки. |
| [DisplayString](./displaystring/) | Получает отображаемую строку, показываемую в MS Excel. Основное отличие от <see cref="DisplayStyle"/> заключается в том, что эта опция также учитывает влияние ширины столбца. Если ширина столбца слишком мала, чтобы полностью показать отформатированную строку, может отображаться "#", как в MS Excel. |
