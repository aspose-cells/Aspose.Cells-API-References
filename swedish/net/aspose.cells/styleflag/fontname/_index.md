---
title: "StyleFlag.FontName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag egenskap. Inställning för fontnamn kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/fontname/
---
## StyleFlag.FontName property

Inställning för teckensnittets namn kommer att tillämpas.

```csharp
public bool FontName { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa exempeldata
            cells["A1"].PutValue("Product Name");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Laptop");
            cells["B2"].PutValue(999.99);
            cells["A3"].PutValue("Phone");
            cells["B3"].PutValue(699.99);

            // Skapa stilar med olika fontnamn
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.Name = "Arial";
            headerStyle.Font.IsBold = true;
            headerStyle.Font.Size = 14;

            Style priceStyle = workbook.CreateStyle();
            priceStyle.Font.Name = "Courier New";
            priceStyle.Custom = "$#,##0.00";

            // Applicera rubrikstil med StyleFlag
            Aspose.Cells.Range headerRange = cells.CreateRange(0, 0, 1, 2);
            StyleFlag headerFlag = new StyleFlag();
            headerFlag.FontName = true;
            headerFlag.FontBold = true;
            headerFlag.FontSize = true;
            headerRange.ApplyStyle(headerStyle, headerFlag);

            // Applicera prisstil med StyleFlag med fokus på FontName
            Aspose.Cells.Range priceRange = cells.CreateRange(1, 1, 2, 1);
            StyleFlag priceFlag = new StyleFlag();
            priceFlag.FontName = true;
            priceFlag.NumberFormat = true;
            priceRange.ApplyStyle(priceStyle, priceFlag);

            // Autoanpassa kolumner för bättre synlighet
            worksheet.AutoFitColumns();

            // Spara arbetsboken
            workbook.Save("FontNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


