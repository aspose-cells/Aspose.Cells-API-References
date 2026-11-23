---
title: "Enum DrawObjectEnum"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Rendering.DrawObjectEnum. Indique Cell ou Image du DrawObject"
type: docs
url: /fr/net/aspose.cells.rendering/drawobjectenum/
---
## DrawObjectEnum enumeration

Indiquer la cellule ou l'image du DrawObject.

```csharp
public enum DrawObjectEnum
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Image | `0` | Indique que DrawObject est une Image |
| Cell | `1` | indique que DrawObject est une Cell |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassDrawObjectEnumDemo
    {
        public static void Run()
        {
            // Créez un classeur et ajoutez des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Cell");

            // Créez un objet PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Créez un DrawObjectEventHandler personnalisé
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Enregistrez le classeur au format PDF avec le gestionnaire personnalisé
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Vérifiez si le draw object est une cell
            if (drawObject.Type == DrawObjectEnum.Cell)
            {
                Cell cell = drawObject.Cell;
                
                // Affichez les informations de la cell
                Console.WriteLine($"Drawing Cell - Row: {cell.Row}, Column: {cell.Column}");
                Console.WriteLine($"Position: ({x}, {y}), Size: {width}x{height}");
                
                // Gestion spéciale pour la cellule A1
                if (cell.Row == 0 && cell.Column == 0)
                {
                    Console.WriteLine("This is cell A1");
                }
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


