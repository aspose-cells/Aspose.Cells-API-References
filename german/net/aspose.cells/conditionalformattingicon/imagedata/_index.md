---
title: "ConditionalFormattingIcon.ImageData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingIcon-Eigenschaft. Gibt die Daten des Symbolsets zurück"
type: docs
url: /de/net/aspose.cells/conditionalformattingicon/imagedata/
---
## ConditionalFormattingIcon.ImageData property

Liefert die Symbolset-Daten.

```csharp
public byte[] ImageData { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten und bedingte Formatierung hinzufügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Ergebnis der bedingten Formatierung abrufen
            var conditionalFormattingResult = worksheet.Cells["A1"].GetConditionalFormattingResult();
            if (conditionalFormattingResult != null)
            {
                ConditionalFormattingIcon icon = conditionalFormattingResult.ConditionalFormattingIcon;
                if (icon != null)
                {
                    // Die Symbol-Bilddaten abrufen
                    byte[] imageData = icon.ImageData;
                    
                    // Überprüfen und Bildinformationen anzeigen
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

### Siehe auch

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


