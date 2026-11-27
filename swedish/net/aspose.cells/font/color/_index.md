---
title: "Font.Color"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar eller anger färgen på teckensnittet"
type: docs
url: /sv/net/aspose.cells/font/color/
---
## Font.Color property

Hämtar eller anger färgen på teckensnittet.

```csharp
public Color Color { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange HTML med olika teckensnittsfärger och -stilar
            Cell cell = worksheet.Cells["A1"];
            cell.HtmlString = "<font color='Red'>Red Text</font> <font color='#0000FF'>Blue Text</font><font style='color:#00FF00;text-decoration: underline;'>Green Underlined</font>";
            
            // Hämta rik textformatering
            FontSetting[] richText = cell.GetCharacters();
            
            // Verifiera och demonstrera färgegenskaper
            Console.WriteLine("First segment color: " + richText[0].Font.Color);
            Console.WriteLine("Second segment color: " + richText[1].Font.Color);
            Console.WriteLine("Third segment underline: " + richText[2].Font.Underline);
            
            // Spara arbetsboken
            workbook.Save("FontColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


