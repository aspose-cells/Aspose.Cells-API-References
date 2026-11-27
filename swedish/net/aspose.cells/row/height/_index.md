---
title: "Row.Height"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-egenskap. Hämtar och anger radens höjd i enheten punkter"
type: docs
url: /sv/net/aspose.cells/row/height/
---
## Row.Height property

Hämtar och anger radens höjd i enheten punkter.

```csharp
public double Height { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyHeightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in radens höjd för den första raden
            Row row = worksheet.Cells.Rows[0];
            row.Height = 30;
            
            // Lägg till lite data i raden
            worksheet.Cells["A1"].PutValue("Row with custom height");
            
            // Verifiera och visa radens höjd
            Console.WriteLine("Row 1 Height: " + row.Height);
            
            // Spara arbetsboken
            workbook.Save("RowHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


