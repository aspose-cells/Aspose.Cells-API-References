---
title: "ConditionalFormattingIcon.GetIconImageData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingIcon-metoden. Hämta ikonuppsättningsdata"
type: docs
url: /sv/net/aspose.cells/conditionalformattingicon/geticonimagedata/
---
## ConditionalFormattingIcon.GetIconImageData method

Hämta ikonuppsättningsdata

```csharp
public static byte[] GetIconImageData(IconSetType type, int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | IconSetType | ikonens typ |
| index | Int32 | ikonens index |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class ConditionalFormattingIconMethodGetIconImageDataWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ingen anledning att skapa en instans eftersom GetIconImageData är statisk
            
            try
            {
                // Anropa GetIconImageData med IconSetType.Arrows3 och index 0
                byte[] imageData = ConditionalFormattingIcon.GetIconImageData(IconSetType.Arrows3, 0);
                
                Console.WriteLine("Method executed successfully. Image data length: " + imageData.Length);
                
                // Spara bilddata till en fil för demonstration
                File.WriteAllBytes("icon_image.png", imageData);
                Console.WriteLine("Icon image saved to icon_image.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetIconImageData method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("ConditionalFormattingIconGetIconImageDataDemo.xlsx");
        }
    }
}
```

### Se även

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


