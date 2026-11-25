---
title: "MsoFormatPicture.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MsoFormatPicture property. Restituisce o imposta il grado di trasparenza dell'area come valore da 0.0 opaco a 1.0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/transparency/
---
## MsoFormatPicture.Transparency property

Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi due immagini al foglio di lavoro
            int index1 = worksheet.Pictures.Add(0, 0, "image1.png");
            int index2 = worksheet.Pictures.Add(2, 0, "image2.png");

            // Imposta la trasparenza per le immagini
            worksheet.Pictures[index1].FormatPicture.Transparency = 0.5;
            worksheet.Pictures[index2].FormatPicture.Transparency = 0.69;

            // Salva e ricarica la cartella di lavoro per verificare le impostazioni di trasparenza
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];

            // Stampa i valori di trasparenza sulla console
            Console.WriteLine("Picture 1 Transparency: " + loadedWorksheet.Pictures[0].FormatPicture.Transparency);
            Console.WriteLine("Picture 2 Transparency: " + loadedWorksheet.Pictures[1].FormatPicture.Transparency);
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


