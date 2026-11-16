---
title: "CellValueType Enum"
linktitle: "CellValueType"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "CellValueType enum. Kapselt das Objekt, das cellvaluetype in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/cellvaluetype/
---

## CellValueType Enum

Gibt einen Zellwerttyp an.

```go

type CellValueType int32


```

## Felder

| Feld | Beschreibung |
| --- | --- |
| [IsUnknown](./isunknown/) | Zellwerttyp ist unbekannt. |
| [IsNull](./isnull/) | Leere Zelle. Der entsprechende Wert sollte null sein. |
| [IsNumeric](./isnumeric/) | Zellwert ist numerisch. Der entsprechende Wert muss int oder double sein. |
| [IsDateTime](./isdatetime/) | Zellwert ist ein Datum/Zeitwert. Der entsprechende Wert muss DateTime sein. |
| [IsString](./isstring/) | Zellwert ist ein String. Der entsprechende Wert muss string sein. |
| [IsBool](./isbool/) | Zellwert ist ein Boolescher Wert. Der entsprechende Wert muss bool sein. |
| [IsError](./iserror/) | Zelle enthält einen Fehlerwert. Der entsprechende Wert muss ein Fehler-String sein. |
