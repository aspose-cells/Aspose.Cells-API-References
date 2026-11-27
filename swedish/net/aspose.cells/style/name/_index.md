---
title: "Style.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar eller anger namnet på stilen"
type: docs
url: /sv/net/aspose.cells/style/name/
---
## Style.Name property

Hämtar eller anger stilens namn.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa och applicera den första namngivna stilen
            Style style1 = workbook.CreateStyle();
            style1.Number = 7;
            style1.Name = "Sales";
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Sales Data");
            
            // Skapa och applicera den andra namngivna stilen
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 14;
            style2.Font.IsBold = true;
            style2.Font.IsItalic = true;
            style2.Font.Color = System.Drawing.Color.Yellow;
            style2.ForegroundColor = System.Drawing.Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            style2.Name = "Header";
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Header Text");
            
            // Spara arbetsboken
            workbook.Save("StylePropertyNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


