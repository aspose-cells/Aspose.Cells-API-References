---
title: "Picture.SourceFullName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Ottiene o imposta il percorso e il nome del file di origine per l'immagine collegata"
type: docs
url: /it/net/aspose.cells.drawing/picture/sourcefullname/
---
## Picture.SourceFullName property

Ottiene o imposta il percorso e il nome del file sorgente per l'immagine collegata.

```csharp
public string SourceFullName { get; set; }
```

### Osservazioni

Il valore predefinito è una stringa vuota. Se SourceFullName non è una stringa vuota, l'immagine è collegata. Se SourceFullName non è una stringa vuota, ma Data è null, allora l'immagine è collegata e non viene memorizzata nel file.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertySourceFullNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine collegata al foglio di lavoro
            string imagePath = "example.png";
            Picture picture = worksheet.Shapes.AddLinkedPicture(0, 0, 100, 100, imagePath);

            // Dimostra la proprietà SourceFullName
            Console.WriteLine("Picture SourceFullName: " + picture.SourceFullName);
            Console.WriteLine("Is linked picture: " + picture.IsLink);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


