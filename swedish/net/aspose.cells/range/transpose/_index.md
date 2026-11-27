---
title: "Range.Transpose"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Transpose roterar data från rader till kolumner eller vice versa"
type: docs
url: /sv/net/aspose.cells/range/transpose/
---
## Range.Transpose method

Transponera (rotera) data från rader till kolumner eller omvänt.

```csharp
public void Transpose()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodTransposeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll exempeldata i ett 3x3-område (A1:C3)
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].PutValue(6);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["C3"].PutValue(9);
            
            // Skapa ett område (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            
            // Transponera området
            range.Transpose();
            
            // Spara arbetsboken
            workbook.Save("TransposedOutput.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


