---
title: "FillFormat.PictureFormatType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Ottiene e imposta il tipo di formato immagine"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/pictureformattype/
---
## FillFormat.PictureFormatType property

Ottiene e imposta il tipo di formato immagine.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare il riempimento dell'immagine
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Imposta le proprietà del riempimento immagine
            shape.Fill.Type = FillType.Texture;
            shape.Fill.Texture = TextureType.BlueTissuePaper;
            shape.Fill.PictureFormatType = FillPictureType.Stretch;

            // Salva la cartella di lavoro
            workbook.Save("FillFormatPictureTypeDemo.xlsx");

            // Carica la cartella di lavoro salvata per verificare le proprietà
            Workbook verifyWorkbook = new Workbook("FillFormatPictureTypeDemo.xlsx");
            Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];

            // Visualizza il PictureFormatType per dimostrarne l'uso
            Console.WriteLine("PictureFormatType: " + verifyShape.Fill.PictureFormatType);
        }
    }
}
```

### Vedi anche

* enum [FillPictureType](../../fillpicturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


