---
title: "CellValue.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellValue-egenskap. Hämtar eller anger cellvärdet"
type: docs
url: /sv/net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

Hämtar eller anger cellvärdet.

```csharp
public object Value { get; set; }
```

### Anmärkningar

Värdet måste vara av rätt objekttyp som motsvarar [`Type`](../type/):

| **Type** | **Value** |
| --- | --- |
| IsNull | null, alla andra objekt kommer att ignoreras |
| IsNumeric | double |
| IsDateTime | DateTime |
| IsString | string |
| IsBool | bool |
| IsError | felsträng såsom "#VALUE!", "#NAME?", ... |

### Exempel

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

### Se även

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


