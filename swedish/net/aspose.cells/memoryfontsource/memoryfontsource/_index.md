---
title: "MemoryFontSource.MemoryFontSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MemoryFontSource-konstruktor. Ctor"
type: docs
url: /sv/net/aspose.cells/memoryfontsource/memoryfontsource/
---
## MemoryFontSource constructor

Konstruktor.

```csharp
public MemoryFontSource(byte[] fontData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontData | Byte[] | Binär typsnittsdata. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourceMethodCtorWithByteArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Läs in en TrueType-typsnittsfil i en bytearray
                byte[] fontData = File.ReadAllBytes("arial.ttf");
                
                // Anropa #ctor-metoden med bytearray-parameter
                MemoryFontSource fontSource = new MemoryFontSource(fontData);
                
                // Ställ in typsnittskällor med den statiska klassen FontConfigs
                FontConfigs.SetFontSources(new FontSourceBase[] { fontSource });
                
                // Verifiera egenskaperna för typsnittskällan
                Console.WriteLine($"Font source type: {fontSource.Type}");
                Console.WriteLine($"Font data length: {fontSource.FontData.Length} bytes");
                
                // Använd typsnittet i en cell
                Worksheet worksheet = workbook.Worksheets[0];
                var style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].PutValue("Text with custom font");
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("MemoryFontSource constructor executed successfully with byte array parameter");
            }
            catch (FileNotFoundException ex)
            {
                Console.WriteLine($"Error: Font file not found. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MemoryFontSource constructor: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("MemoryFontSourceCtorDemo.xlsx");
        }
    }
}
```

### Se även

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


