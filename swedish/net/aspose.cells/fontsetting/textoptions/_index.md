---
title: "FontSetting.TextOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSetting-egenskap. Returnerar textalternativen"
type: docs
url: /sv/net/aspose.cells/fontsetting/textoptions/
---
## FontSetting.TextOptions property

Returnerar textalternativen.

```csharp
public TextOptions TextOptions { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeltext med olika formateringssektioner
            string part1 = "This is normal text. ";
            string part2 = "This is bold and italic text. ";
            string part3 = "This is normal again. ";
            string part4 = "This is bold text.";
            
            // Kombinera alla delar till en cell
            Cell cell = worksheet.Cells["A1"];
            cell.Value = part1 + part2 + part3 + part4;
            
            // Tillämpa formatering på specifika delar av texten
            int startPos1 = part1.Length;
            int length1 = part2.Length;
            cell.Characters(startPos1, length1).TextOptions.IsBold = true;
            cell.Characters(startPos1, length1).TextOptions.IsItalic = true;
            
            int startPos2 = part1.Length + part2.Length + part3.Length;
            int length2 = part4.Length;
            cell.Characters(startPos2, length2).TextOptions.IsBold = true;
            
            // Spara arbetsboken
            workbook.Save("TextOptionsDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("TextOptions demo completed. File saved.");
        }
    }
}
```

### Se även

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


