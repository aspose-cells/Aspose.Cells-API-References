---
title: "Worksheet.BackgroundImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene e imposta l'immagine di sfondo del foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/backgroundimage/
---
## Worksheet.BackgroundImage property

Ottiene e imposta l'immagine di sfondo del foglio di lavoro.

```csharp
public byte[] BackgroundImage { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyBackgroundImageDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni il primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Percorso del file immagine
            string imagePath = "background.jpg";
            
            // Leggi il file immagine in un array di byte
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Imposta l'immagine di sfondo per il foglio di lavoro
            worksheet.BackgroundImage = imageData;
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetWithBackground.xlsx");
            
            Console.WriteLine("Worksheet background image set successfully.");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


