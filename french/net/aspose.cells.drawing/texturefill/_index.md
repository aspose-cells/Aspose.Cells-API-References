---
title: "Classe TextureFill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.TextureFill. Encapsule l'objet qui représente le format de remplissage de texture"
type: docs
url: /fr/net/aspose.cells.drawing/texturefill/
---
## TextureFill class

Encapsule l'objet qui représente le format de remplissage de texture.

```csharp
public class TextureFill : Fill
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ImageData](../../aspose.cells.drawing/texturefill/imagedata/) { get; set; } | Obtient et définit les données d'image du remplissage. |
| [IsTiling](../../aspose.cells.drawing/texturefill/istiling/) { get; set; } | Indique si l'image est utilisée comme texture en mosaïque. |
| [PicFormatOption](../../aspose.cells.drawing/texturefill/picformatoption/) { get; set; } | Obtient ou définit l'option de format d'image. |
| [PictureFormatType](../../aspose.cells.drawing/texturefill/pictureformattype/) { get; set; } | Obtient et définit le type de format d'image. |
| [Scale](../../aspose.cells.drawing/texturefill/scale/) { get; set; } | Obtient et définit l'échelle du format d'image. |
| [TilePicOption](../../aspose.cells.drawing/texturefill/tilepicoption/) { get; set; } | Obtient ou définit l'option d'image en mosaïque. |
| [Transparency](../../aspose.cells.drawing/texturefill/transparency/) { get; set; } | Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [Type](../../aspose.cells.drawing/texturefill/type/) { get; set; } | Obtient et définit le type de texture |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Hérité de [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Obtient le code de hachage.(Hérité de [`Fill`](../fill/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassTextureFillDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez une forme rectangulaire pour démontrer le remplissage de texture
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 150, 300);
            
            // Appliquez le remplissage de texture à la forme et obtenez l'instance existante de TextureFill
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;
            
            // Définissez le type de texture intégré
            textureFill.Type = TextureType.BlueTissuePaper;
            
            // Configurez les options de mosaïquage
            textureFill.IsTiling = true;
            TilePicOption tileOptions = new TilePicOption
            {
                ScaleX = 0.5,
                ScaleY = 0.5,
                OffsetX = 10,
                OffsetY = 10
            };
            textureFill.TilePicOption = tileOptions;
            
            // Définissez la transparence et le redimensionnement du remplissage
            textureFill.Transparency = 0.2;
            textureFill.Scale = 0.8;
            
            // Enregistrez le classeur avec le remplissage de texture appliqué
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


