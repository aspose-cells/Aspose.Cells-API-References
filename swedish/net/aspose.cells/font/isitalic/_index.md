---
title: "Font.IsItalic"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar eller anger ett värde som indikerar om fonten är kursiv"
type: docs
url: /sv/net/aspose.cells/font/isitalic/
---
## Font.IsItalic property

Hämtar eller anger ett värde som indikerar om teckensnittet är kursivt.

```csharp
public bool IsItalic { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsItalicDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt standardstilen
            Style style = workbook.DefaultStyle;
            
            // Ange font-egenskaper inklusive IsItalic
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.Font.IsItalic = true;
            
            // Applicera stilen på cell A1
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Italic Text Example");
            
            // Spara arbetsboken
            workbook.Save("FontPropertyIsItalicDemo.xlsx");
            
            // Verifiera den kursiva egenskapen
            Console.WriteLine("Font is italic: " + cell.GetStyle().Font.IsItalic);
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


