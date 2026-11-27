---
title: "Worksheet.AutoFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑egenskap. Representerar autofilter för det angivna arbetsbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/autofilter/
---
## Worksheet.AutoFilter property

Representerar autofilter för det angivna kalkylbladet.

```csharp
public AutoFilter AutoFilter { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Shirt");
            worksheet.Cells["B3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Phone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["A5"].PutValue("Pants");
            worksheet.Cells["B5"].PutValue("Clothing");

            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.Filter(1, "Electronics");

            // Uppdatera filtret
            worksheet.AutoFilter.Refresh();

            // Spara arbetsboken
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


