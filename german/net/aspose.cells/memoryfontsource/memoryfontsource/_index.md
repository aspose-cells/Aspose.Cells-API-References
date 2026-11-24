---
title: "MemoryFontSource.MemoryFontSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MemoryFontSource-Konstruktor. Ctor"
type: docs
url: /de/net/aspose.cells/memoryfontsource/memoryfontsource/
---
## MemoryFontSource constructor

Ctor.

```csharp
public MemoryFontSource(byte[] fontData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontData | Byte[] | Binäre Schriftartdaten. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Laden Sie eine TrueType-Schriftdatei in ein Byte-Array
                byte[] fontData = File.ReadAllBytes("arial.ttf");
                
                // Rufen Sie die #ctor-Methode mit einem Byte-Array-Parameter auf
                MemoryFontSource fontSource = new MemoryFontSource(fontData);
                
                // Schriftquellen mit der statischen Klasse FontConfigs festlegen
                FontConfigs.SetFontSources(new FontSourceBase[] { fontSource });
                
                // Überprüfen Sie die Eigenschaften der Schriftquelle
                Console.WriteLine($"Font source type: {fontSource.Type}");
                Console.WriteLine($"Font data length: {fontSource.FontData.Length} bytes");
                
                // Verwenden Sie die Schriftart in einer Zelle
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
            
            // Ergebnis speichern
            workbook.Save("MemoryFontSourceCtorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


