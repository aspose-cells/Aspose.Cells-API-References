---
title: "OleObject.ImageSourceFullName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Ottiene o imposta il percorso e il nome del file sorgente per l'immagine collegata"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/imagesourcefullname/
---
## OleObject.ImageSourceFullName property

Ottiene o imposta il percorso e il nome del file sorgente per l'immagine collegata.

```csharp
public string ImageSourceFullName { get; set; }
```

### Osservazioni

Il valore predefinito è una stringa vuota. Se SourceFullName non è una stringa vuota, l'immagine è collegata. Se SourceFullName non è una stringa vuota, ma Data è null, allora l'immagine è collegata e non viene memorizzata nel file.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageSourceFullNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // File PDF di esempio da incorporare
            byte[] pdfBytes = File.ReadAllBytes("example.pdf");

            // Aggiungi un OleObject al foglio di lavoro
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfBytes);
            OleObject oleObj = worksheet.OleObjects[oleIndex];

            // Imposta le proprietà OleObject includendo ImageSourceFullName
            oleObj.DisplayAsIcon = false;
            oleObj.FileFormatType = FileFormatType.Pdf;
            oleObj.ImageSourceFullName = "sample_image.png"; // Demonstrating ImageSourceFullName usage
            oleObj.IsAutoSize = false;
            oleObj.IsLink = false;
            oleObj.ProgID = "Acrobat.Document.DC";

            // Salva la cartella di lavoro
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


