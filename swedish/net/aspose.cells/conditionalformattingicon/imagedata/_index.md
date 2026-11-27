---
title: "ConditionalFormattingIcon.ImageData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingIcon-egenskapen. Hämtar ikonuppsättningsdata"
type: docs
url: /sv/net/aspose.cells/conditionalformattingicon/imagedata/
---
## ConditionalFormattingIcon.ImageData property

Hämtar ikonuppsättningsdata.

```csharp
public byte[] ImageData { get; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyImageDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och villkorsstyrd formatering
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Hämta resultatet av villkorsstyrd formatering
            var conditionalFormattingResult = worksheet.Cells["A1"].GetConditionalFormattingResult();
            if (conditionalFormattingResult != null)
            {
                ConditionalFormattingIcon icon = conditionalFormattingResult.ConditionalFormattingIcon;
                if (icon != null)
                {
                    // Hämta ikonens bilddata
                    byte[] imageData = icon.ImageData;
                    
                    // Verifiera och visa bildinformation
                    if (imageData != null && imageData.Length > 0)
                    {
                        Console.WriteLine($"Icon data length: {imageData.Length} bytes");
                    }
                }
            }
        }
    }
}
```

### Se även

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


