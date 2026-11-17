---
title: "Перечисление TxtLoadStyleStrategy"
linktitle: "TxtLoadStyleStrategy"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление TxtLoadStyleStrategy. Инкапсулирует объект, представляющий txtloadstylestrategy в Go."
type: docs
weight: 200
url: /ru/go-cpp/txtloadstylestrategy/
---

## TxtLoadStyleStrategy Enum

Указывает, как применять стиль к разобранным значениям при преобразовании строкового значения в число или дату/время.

```go

type TxtLoadStyleStrategy int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [None](./none/) | Не задает стиль для разобранного значения. |
| [BuiltIn](./builtin/) | Устанавливает стиль как встроенный номер/дата‑время, когда разобранное значение является простым числом/датой‑временем. |
| [ExactFormat](./exactformat/) | Устанавливает точный пользовательский формат для разобранного значения, чтобы отформатированное значение совпадало с оригинальным вводом. |
