---
title: "Classe PicFormatOption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.PicFormatOption class. Rappresenta l'opzione di formato immagine."
type: docs
url: /it/net/aspose.cells.drawing/picformatoption/
---
## PicFormatOption class

Rappresenta l'opzione di formato immagine

```csharp
public class PicFormatOption
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PicFormatOption](picformatoption/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Bottom](../../aspose.cells.drawing/picformatoption/bottom/) { get; set; } | Ottiene o imposta lo spostamento inferiore per lo stretching dell'immagine. |
| [Left](../../aspose.cells.drawing/picformatoption/left/) { get; set; } | Ottiene o imposta lo spostamento sinistro per lo stretching dell'immagine. |
| [Right](../../aspose.cells.drawing/picformatoption/right/) { get; set; } | Ottiene o imposta lo spostamento destro per lo stretching dell'immagine. |
| [Scale](../../aspose.cells.drawing/picformatoption/scale/) { get; set; } | Ottiene o imposta il numero di stack dell'immagine e la scala associata. |
| [Top](../../aspose.cells.drawing/picformatoption/top/) { get; set; } | Ottiene o imposta lo spostamento superiore per lo stretching dell'immagine. |
| [Type](../../aspose.cells.drawing/picformatoption/type/) { get; set; } | Ottiene o imposta il tipo di riempimento dell'immagine. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.IO;

    public class DrawingClassPicFormatOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma e imposta il riempimento dell'immagine
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);
            // Proprietà FillType rimossa dall'accesso a MsoFillFormat
            shape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");

            // Configura le opzioni del formato immagine
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.15,
                Right = 0.15,
                Top = 0.15,
                Bottom = 0.15,
                Scale = 0.8
            };

            // Aggiungi una seconda forma con immagine a mosaico
            Shape tiledShape = worksheet.Shapes.AddRectangle(5, 210, 0, 0, 200, 200);
            // Proprietà FillType rimossa dall'accesso a MsoFillFormat
            tiledShape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");
            
            PicFormatOption tileFormat = new PicFormatOption
            {
                Type = FillPictureType.Stack,
                Scale = 1.5
            };

            workbook.Save("PicFormatOptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


