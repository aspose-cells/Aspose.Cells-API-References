---
title: "Cell.Worksheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar det överordnade kalkylbladet"
type: docs
url: /sv/net/aspose.cells/cell/worksheet/
---
## Cell.Worksheet property

Hämtar det överordnade kalkylbladet.

```csharp
public Worksheet Worksheet { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Åtkomst till en cell och demonstrera Worksheet-egenskapen
            Cell cell = worksheet.Cells["A3"];
            
            // Visa kalkylbladsinformation via cellens Worksheet-egenskap
            Console.WriteLine("Cell A3 is in worksheet: " + cell.Worksheet.Name);
            Console.WriteLine("Calculation result in A3: " + cell.Value);
            
            // Lägg till ett annat kalkylblad och demonstrera korsreferens mellan blad
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=A3");
            
            // Åtkomst till cellen i Sheet2 och visa dess kalkylblad
            Cell crossSheetCell = sheet2.Cells["B1"];
            Console.WriteLine("Cell B1 is in worksheet: " + crossSheetCell.Worksheet.Name);
            Console.WriteLine("Cross-sheet reference in B1: " + crossSheetCell.Value);
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


