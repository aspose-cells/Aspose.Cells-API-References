---
title: "CellValueType Enum"
linktitle: "CellValueType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "CellValueType enum. Inkapslar objektet som representerar cellvaluetype i Go."
type: docs
weight: 200
url: /sv/go-cpp/cellvaluetype/
---

## CellValueType Enum

Anger en cellvärdestyp.

```go

type CellValueType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [IsUnknown](./isunknown/) | Cellvärdestyp är okänd. |
| [IsNull](./isnull/) | Tom cell. Tillhörande värde bör vara null. |
| [IsNumeric](./isnumeric/) | Cellvärdet är numeriskt. Tillhörande värde måste vara int eller double. |
| [IsDateTime](./isdatetime/) | Cellvärdet är datum/tid. Tillhörande värde måste vara DateTime. |
| [IsString](./isstring/) | Cellvärdet är en sträng. Tillhörande värde måste vara en sträng. |
| [IsBool](./isbool/) | Cellvärdet är booleskt. Tillhörande värde måste vara bool. |
| [IsError](./iserror/) | Cellen innehåller felvärde. Tillhörande värde måste vara felsträng. |
