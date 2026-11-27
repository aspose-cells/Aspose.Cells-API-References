---
title: "PageSetup.PrintTitleRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar raderna som innehåller cellerna som ska upprepas högst upp på varje sida"
type: docs
url: /sv/net/aspose.cells/pagesetup/printtitlerows/
---
## PageSetup.PrintTitleRows property

Anger de rader som innehåller cellerna som ska upprepas högst upp på varje sida.

```csharp
public string PrintTitleRows { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleRowsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange några exempeldata
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Data " + (i-1));
            }
            
            // Kom åt sidinställning
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ställ in utskriftsrubrikrader (första raden kommer att upprepas på varje utskriven sida)
            pageSetup.PrintTitleRows = "$1:$1";
            
            // Spara arbetsboken
            workbook.Save("PrintTitleRowsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


