---
title: "Enum PasteOperationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PasteOperationType-enumen. Representerar operationstypen när ett område klistras in"
type: docs
url: /sv/net/aspose.cells/pasteoperationtype/
---
## PasteOperationType enumeration

Representerar operationstypen när ett område klistras in.

```csharp
public enum PasteOperationType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen operation. |
| Add | `1` | Lägg till |
| Subtract | `2` | Subtrahera |
| Multiply | `3` | Multiplicera |
| Divide | `4` | Dela |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPasteOperationTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["B1"].PutValue(20);
            sheet.Cells["C1"].PutValue(30);
            
            // Skapa inklistringsalternativ med PasteOperationType.None
            var pasteOptions = new PasteOptions()
            {
                PasteType = PasteType.Values,
                OperationType = PasteOperationType.None,
                SkipBlanks = false,
                Transpose = false
            };

            // Skapa område och kopiera med inklistringsalternativ
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1", "C1");
            Aspose.Cells.Range destRange = sheet.Cells.CreateRange("A2", "C2");
            sourceRange.Copy(destRange, pasteOptions);

            // Spara arbetsboken
            workbook.Save("PasteOperationTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


