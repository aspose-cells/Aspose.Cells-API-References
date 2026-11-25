---
title: "Picture.DisplayAsIcon"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Picture. Vero se l'oggetto specificato è visualizzato come icona e l'immagine non verrà modificata automaticamente"
type: docs
url: /it/net/aspose.cells.drawing/picture/displayasicon/
---
## Picture.DisplayAsIcon property

True se l'oggetto specificato è visualizzato come icona e l'immagine non verrà modificata automaticamente.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.ico");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Imposta la proprietà DisplayAsIcon su vero
            picture.DisplayAsIcon = true;
            
            // Imposta altre proprietà picture
            picture.Name = "IconDisplay";
            picture.Height = 100;
            picture.Width = 100;

            // Salva la cartella di lavoro
            workbook.Save("DisplayAsIconDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon display picture.");
        }
    }
}
```

### Vedi anche

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


