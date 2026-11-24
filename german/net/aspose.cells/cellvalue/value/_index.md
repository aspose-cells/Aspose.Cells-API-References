---
title: "CellValue.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellValue‑Eigenschaft. Liest oder setzt den Zellenwert"
type: docs
url: /de/net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

Liest oder setzt den Zellenwert.

```csharp
public object Value { get; set; }
```

### Hinweise

Der Wert muss vom korrekten Objekttyp sein, der dem [`Type`](../type/)-Typ entspricht:

| **Type** | **Value** |
| --- | --- |
| IsNull | null, jedes andere Objekt wird ignoriert |
| IsNumeric | double |
| IsDateTime | DateTime |
| IsString | string |
| IsBool | bool |
| IsError | Fehlerzeichenkette wie "#VALUE!", "#NAME?", ... |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            worksheet.Cells["A1"].PutValue(cellValue.Value);

            workbook.Save("CellValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


