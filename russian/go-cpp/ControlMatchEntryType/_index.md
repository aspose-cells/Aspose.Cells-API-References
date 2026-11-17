---
title: "Перечисление ControlMatchEntryType"
linktitle: "ControlMatchEntryType"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Перечисление ControlMatchEntryType. Инкапсулирует объект, представляющий controlmatchentrytype в Go."
type: docs
weight: 200
url: /ru/go-cpp/controlmatchentrytype/
---

## ControlMatchEntryType Enum

Представляет способ, которым ListBox или ComboBox ищет в списке при вводе пользователем.

```go

type ControlMatchEntryType int32


```

## Поля

| Поле | Описание |
| --- | --- |
| [FirstLetter](./firstletter/) | Элемент управления ищет следующую запись, начинающуюся с введённого символа. При повторном вводе той же буквы происходит переключение между всеми записями, начинающимися с этой буквы. |
| [Complete](./complete/) | По мере ввода каждого символа элемент управления ищет запись, соответствующую всем введённым символам. |
| [None](./none/) | Список не будет просматриваться при вводе символов. |
