---
title: "FontConfigs.GetFontFileDataInfo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontConfigs-metod. Hämta datainformation om teckensnittfilens data"
type: docs
url: /sv/net/aspose.cells/fontconfigs/getfontfiledatainfo/
---
## FontConfigs.GetFontFileDataInfo method

Hämta datainformation för teckensnittsfilens data.

```csharp
public static FontFileDataInfo GetFontFileDataInfo(string fontName, bool isBold, bool isItalic, 
    bool isExactStyle)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontName | String | teckensnittsnamn |
| isBold | Boolean | teckensnittsstilen är fet eller inte |
| isItalic | Boolean | teckensnittsstilen är kursiv eller inte |
| isExactStyle | Boolean | om den angivna fet/kursiv-stilen ska matchas exakt |

### Returvärde

Datainformation om teckensnittfilens data.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontFileDataInfoWithStringBooleanBooleanBooleanDemo
    {
        public static void Run()
        {
            try
            {
                // Anropa GetFontFileDataInfo med specifika parametrar (ändrad till statiskt anrop)
                FontFileDataInfo fontInfo = FontConfigs.GetFontFileDataInfo("Arial", true, false, false);

                // Visa information om teckensnittfilens data
                if (fontInfo != null)
                {
                    Console.WriteLine($"Font format type: {fontInfo.FormatType}");
                    Console.WriteLine($"Font data length: {fontInfo.Data?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Font information not available");
                }

                // Visa effekten på en arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Ställ in stil med teckensnittet vi kontrollerade
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.IsBold = true;
                style.Font.IsItalic = false;
                
                // Applicera stil på en cell
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with Arial Bold");

                // Spara arbetsboken
                workbook.Save("FontConfigsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontFileDataInfo method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [FontFileDataInfo](../../fontfiledatainfo/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


