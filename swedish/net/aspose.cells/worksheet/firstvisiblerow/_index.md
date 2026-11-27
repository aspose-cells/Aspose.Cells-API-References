---
title: "Worksheet.FirstVisibleRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Representerar index för den första synliga raden"
type: docs
url: /sv/net/aspose.cells/worksheet/firstvisiblerow/
---
## Worksheet.FirstVisibleRow property

Representerar första synliga radens index.

```csharp
public int FirstVisibleRow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange några exempeldata
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Ställ in den första synliga raden till rad 20
            worksheet.FirstVisibleRow = 20;
            
            // Visa den första synliga raden
            Console.WriteLine("First visible row: " + worksheet.FirstVisibleRow);
            
            // Spara arbetsboken
            workbook.Save("FirstVisibleRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


