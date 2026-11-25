---
title: "MsoFormatPicture.IsGray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFormatPicture. Indica se quest'immagine deve essere visualizzata in scala di grigi"
type: docs
url: /it/net/aspose.cells.drawing/msoformatpicture/isgray/
---
## MsoFormatPicture.IsGray property

Indica se questa immagine deve essere visualizzata in scala di grigi.

```csharp
public bool IsGray { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsGrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma immagine
            using (Stream imageStream = File.OpenRead("example.gif"))
            {
                Shape shape = worksheet.Shapes.AddPicture(0, 0, imageStream, 100, 100);
                
                // Imposta le proprietà del formato immagine
                shape.FormatPicture.Brightness = 90;
                shape.FormatPicture.Contrast = 90;
                shape.FormatPicture.IsGray = true;

                // Salva la cartella di lavoro
                workbook.Save("output.xlsx");
            }

            // Ricarica e verifica le proprietà
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Brightness: " + loadedShape.FormatPicture.Brightness);
            Console.WriteLine("Contrast: " + loadedShape.FormatPicture.Contrast);
            Console.WriteLine("IsGray: " + loadedShape.FormatPicture.IsGray);
        }
    }
}
```

### Vedi anche

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


