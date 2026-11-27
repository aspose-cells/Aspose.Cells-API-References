---
title: "Font.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar eller anger namnet på Font"
type: docs
url: /sv/net/aspose.cells/font/name/
---
## Font.Name property

Hämtar eller anger namnet på [`Font`](../).

```csharp
public virtual string Name { get; set; }
```

### Anmärkningar

Om den här egenskapen används för att ange namnet på teckensnittet, kommer [`SchemeType`](../schemetype/) att uppdateras till None

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt standardarbetsbladet och cellerna
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Skapa och ändra en stil med font-egenskaper
            Style style = workbook.CreateStyle();
            Font font = style.Font;
            
            // Demonstrera användning av Name‑egenskapen
            font.Name = "Arial";  // Changed from FontNameConstants.Arial to string literal
            font.Size = 14;
            font.IsBold = true;
            
            // Tillämpa stilen på en cell
            cells["A1"].PutValue("Font Property Name Demo");
            cells["A1"].SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("FontPropertyNameDemo.xlsx");
            
            Console.WriteLine("Demo completed. File saved as FontPropertyNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


