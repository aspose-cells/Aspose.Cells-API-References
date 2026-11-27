---
title: "Font.Size"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar eller anger storleken på teckensnittet"
type: docs
url: /sv/net/aspose.cells/font/size/
---
## Font.Size property

Hämtar eller anger storleken på teckensnittet.

```csharp
public int Size { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in text med olika teckensnittsstorlekar
            Cell cell1 = worksheet.Cells["A1"];
            cell1.Value = "Text with size 12";
            Style style1 = workbook.CreateStyle();
            style1.Font.Size = 12;
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A3"];
            cell2.Value = "Text with size 16";
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 16;
            cell2.SetStyle(style2);

            // Spara arbetsboken
            workbook.Save("FontSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


