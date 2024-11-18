---
title: ControlMatchEntryType Enum 
linktitle: ControlMatchEntryType
second_title: Aspose.Cells for Go API Reference
description: 'ControlMatchEntryType enum. Encapsulates the object that represents controlmatchentrytype in Go.'
type: docs
weight: 200
url: /go/aspose.cells.drawing.activexcontrols/controlmatchentrytype/
---

## ControlMatchEntryType Enum

Represents how a ListBox or ComboBox searches its list as the user types.

```go

type ControlMatchEntryType int32


```

## Fields

| Field | Description |
| --- | --- |
|[FirstLetter](./firstletter/) | The control searches for the next entry that starts with the character entered.Repeatedly typing the same letter cycles through all entries beginning with that letter. | 
|[Complete](./complete/) | As each character is typed, the control searches for an entry matching all characters entered. | 
|[None](./none/) | The list will not be searched when characters are typed. | 
