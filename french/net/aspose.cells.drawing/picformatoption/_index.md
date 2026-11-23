---
title: "Classe PicFormatOption"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.PicFormatOption class. Représente l'option de format d'image."
type: docs
url: /fr/net/aspose.cells.drawing/picformatoption/
---
## PicFormatOption class

Représente l'option de format d'image

```csharp
public class PicFormatOption
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PicFormatOption](picformatoption/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Bottom](../../aspose.cells.drawing/picformatoption/bottom/) { get; set; } | Obtient ou définit le décalage inférieur pour l'étirement de l'image. |
| [Left](../../aspose.cells.drawing/picformatoption/left/) { get; set; } | Obtient ou définit le décalage gauche pour l'étirement de l'image. |
| [Right](../../aspose.cells.drawing/picformatoption/right/) { get; set; } | Obtient ou définit le décalage droit pour l'étirement de l'image. |
| [Scale](../../aspose.cells.drawing/picformatoption/scale/) { get; set; } | Obtient ou définit le nombre d'empilements et d'échelles de l'image. |
| [Top](../../aspose.cells.drawing/picformatoption/top/) { get; set; } | Obtient ou définit le décalage supérieur pour l'étirement de l'image. |
| [Type](../../aspose.cells.drawing/picformatoption/type/) { get; set; } | Obtient ou définit le type de remplissage de l'image. |

### Exemples

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

            // Ajouter une forme et définir le remplissage d'image
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);
            // Propriété FillType supprimée de l'accès MsoFillFormat
            shape.FillFormat.ImageData = File.ReadAllBytes("aspose-logo.png");

            // Configurer les options de format d'image
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.15,
                Right = 0.15,
                Top = 0.15,
                Bottom = 0.15,
                Scale = 0.8
            };

            // Ajouter une deuxième forme avec une image en mosaïque
            Shape tiledShape = worksheet.Shapes.AddRectangle(5, 210, 0, 0, 200, 200);
            // Propriété FillType supprimée de l'accès MsoFillFormat
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

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


