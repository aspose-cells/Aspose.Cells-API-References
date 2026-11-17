---
title: "Перечисление CellValueType"
linktitle: "CellValueType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление CellValueType. Инкапсулирует объект, представляющий cellvaluetype в Go."
type: docs
weight: 200
url: /ru/go-cpp/cellvaluetype/
---

## CellValueType Enum

Указывает тип значения ячейки.

```go

type CellValueType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [IsUnknown](./isunknown/) | Тип значения ячейки неизвестен. |
| [IsNull](./isnull/) | Пустая ячейка. Соответствующее значение должно быть null. |
| [IsNumeric](./isnumeric/) | Значение ячейки числовое. Соответствующее значение должно быть int или double. |
| [IsDateTime](./isdatetime/) | Значение ячейки — дата и время. Соответствующее значение должно быть DateTime. |
| [IsString](./isstring/) | Значение ячейки — строка. Соответствующее значение должно быть string. |
| [IsBool](./isbool/) | Значение ячейки — логическое. Соответствующее значение должно быть bool. |
| [IsError](./iserror/) | Ячейка содержит значение ошибки. Соответствующее значение должно быть строкой ошибки. |
