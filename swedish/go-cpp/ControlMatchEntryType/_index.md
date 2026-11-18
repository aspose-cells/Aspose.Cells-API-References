---
title: "ControlMatchEntryType Enum"
linktitle: "ControlMatchEntryType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ControlMatchEntryType enum. Inkapslar objektet som representerar controlmatchentrytype i Go."
type: docs
weight: 200
url: /sv/go-cpp/controlmatchentrytype/
---

## ControlMatchEntryType Enum

Representerar hur en ListBox eller ComboBox söker i sin lista när användaren skriver.

```go

type ControlMatchEntryType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [FirstLetter](./firstletter/) | Kontrollen söker efter nästa post som börjar med det angivna tecknet. Att upprepade gånger skriva samma bokstav cyklar igenom alla poster som börjar med den bokstaven. |
| [Complete](./complete/) | När varje tecken skrivs in söker kontrollen efter en post som matchar alla inmatade tecken. |
| [None](./none/) | Listan kommer inte att sökas när tecken skrivs in. |
