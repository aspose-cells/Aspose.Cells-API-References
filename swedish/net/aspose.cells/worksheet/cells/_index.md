---
title: "Worksheet.Cells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar Cells-samlingen"
type: docs
url: /sv/net/aspose.cells/worksheet/cells/
---
## Worksheet.Cells property

Hämtar [`Cells`](../../cells/) samlingen.

```csharp
public Cells Cells { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cells-samlingen
            Cells cells = worksheet.Cells;
            
            // Ange värden i cells
            cells["A1"].PutValue("Item");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);
            
            // Ange formel för att beräkna totalen
            cells["A4"].PutValue("Total:");
            cells["B4"].Formula = "=SUM(B2:B3)";
            
            // Beräkna formler
            workbook.CalculateFormula();
            
            // Visa cellvärden
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);
            Console.WriteLine("B2: " + cells["B2"].StringValue);
            Console.WriteLine("A3: " + cells["A3"].StringValue);
            Console.WriteLine("B3: " + cells["B3"].StringValue);
            Console.WriteLine("A4: " + cells["A4"].StringValue);
            Console.WriteLine("B4: " + cells["B4"].StringValue + " (Formula: " + cells["B4"].Formula + ")");
            
            // Spara arbetsbok
            workbook.Save("CellsPropertyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cells](../../cells/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


