---
title: "Klasse PicFormatOption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.PicFormatOption Klasse. Stellt die Bildformatoption dar"
type: docs
url: /de/net/aspose.cells.drawing/picformatoption/
---
## PicFormatOption class

Stellt die Bildformatoption dar

```csharp
public class PicFormatOption
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PicFormatOption](picformatoption/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Bottom](../../aspose.cells.drawing/picformatoption/bottom/) { get; set; } | Liest oder legt den unteren Versatz für das Dehnen des Bildes fest. |
| [Left](../../aspose.cells.drawing/picformatoption/left/) { get; set; } | Liest oder legt den linken Versatz für das Dehnen des Bildes fest. |
| [Right](../../aspose.cells.drawing/picformatoption/right/) { get; set; } | Liest oder legt den rechten Versatz für das Dehnen des Bildes fest. |
| [Scale](../../aspose.cells.drawing/picformatoption/scale/) { get; set; } | Liest oder legt fest, wie viele das Bild stapelt und mit welchem Maßstab. |
| [Top](../../aspose.cells.drawing/picformatoption/top/) { get; set; } | Liest oder legt den oberen Versatz für das Dehnen des Bildes fest. |
| [Type](../../aspose.cells.drawing/picformatoption/type/) { get; set; } | Liest oder legt den Bildfülltyp fest. |

### Beispiele

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

            // Füge eine Form hinzu und setze die Bildfüllung
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);
            // FillType-Eigenschaft aus dem Zugriff auf MsoFillFormat entfernt
            shape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");

            // Bildformatoptionen konfigurieren
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.15,
                Right = 0.15,
                Top = 0.15,
                Bottom = 0.15,
                Scale = 0.8
            };

            // Füge eine zweite Form mit gekacheltem Bild hinzu
            Shape tiledShape = worksheet.Shapes.AddRectangle(5, 210, 0, 0, 200, 200);
            // FillType-Eigenschaft aus dem Zugriff auf MsoFillFormat entfernt
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

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


