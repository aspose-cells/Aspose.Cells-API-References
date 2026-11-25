---
title: "ConditionalFormattingIcon.ImageData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConditionalFormattingIcon. Ottiene i dati del set di icone"
type: docs
url: /it/net/aspose.cells/conditionalformattingicon/imagedata/
---
## ConditionalFormattingIcon.ImageData property

Ottiene i dati del set di icone.

```csharp
public byte[] ImageData { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio e formattazione condizionale
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Ottieni il risultato della formattazione condizionale
            var conditionalFormattingResult = worksheet.Cells["A1"].GetConditionalFormattingResult();
            if (conditionalFormattingResult != null)
            {
                ConditionalFormattingIcon icon = conditionalFormattingResult.ConditionalFormattingIcon;
                if (icon != null)
                {
                    // Ottieni i dati dell'immagine dell'icona
                    byte[] imageData = icon.ImageData;
                    
                    // Verifica e visualizza le informazioni dell'immagine
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

### Vedi anche

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


