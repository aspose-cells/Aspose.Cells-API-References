---
title: "Cell.IsRichText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cellmetod. Anger om cellens strängvärde är rik formaterad text"
type: docs
url: /sv/net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

Indikerar om strängvärdet i den här cellen är en rik formaterad text.

```csharp
public bool IsRichText()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodIsRichTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en cell med rik textformatering
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello World");
            
            // Applicera rik textformatering
            FontSetting boldFont = cell.GetCharacters()[0];
            boldFont.Font.IsBold = true;
            
            FontSetting normalFont = cell.GetCharacters()[6];
            normalFont.Font.IsBold = false;
            
            // Kontrollera om cellen innehåller rik text
            bool isRichText = cell.IsRichText();
            Console.WriteLine("Is cell A1 rich text? " + isRichText);
            
            // Spara arbetsboken
            workbook.Save("RichTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


