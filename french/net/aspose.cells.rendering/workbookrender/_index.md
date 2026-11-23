---
title: "Classe WorkbookRender"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.WorkbookRender. Représente le rendu d’un classeur. Le constructeur de cette classe doit être utilisé après la modification du style de cellule de la configuration de page"
type: docs
url: /fr/net/aspose.cells.rendering/workbookrender/
---
## WorkbookRender class

Représente un rendu de classeur. Le constructeur de cette classe doit être utilisé après la modification de la configuration de page, du style de cellule.

```csharp
public class WorkbookRender
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WorkbookRender](workbookrender/)(Workbook, ImageOrPrintOptions) | La construction de WorkbookRender |

## Propriétés

| Nom | Description |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/workbookrender/pagecount/) { get; } | Obtient le nombre total de pages du classeur. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/workbookrender/customprint/)(bool, PrintPageEventArgs) | Le client peut contrôler les paramètres de page de l’imprimante lors de l’impression de chaque page à l’aide de cette fonction. |
| [Dispose](../../aspose.cells.rendering/workbookrender/dispose/)() | Libère les ressources créées et utilisées pour le rendu. |
| [GetPageSizeInch](../../aspose.cells.rendering/workbookrender/getpagesizeinch/)(int) | Obtenir la taille de page en pouces de l’image de sortie. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage)(int) | Rendre une page donnée vers un objet Bitmap. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_3)(Stream) | Rendre l’ensemble du classeur en tant qu’image Tiff vers un flux. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_4)(string) | Rendre l’ensemble du classeur en tant qu’image Tiff vers un fichier. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_1)(int, Stream) | Rendre une page donnée vers un flux. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_2)(int, string) | Rendre une page donnée vers un fichier. |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter)(PrinterSettings) | Rendre le classeur vers l’imprimante |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_2)(string) | Rendre le classeur vers l’imprimante |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_1)(PrinterSettings, string) | Rendre le classeur vers l’imprimante |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_4)(string, string) | Rendre le classeur vers l’imprimante |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Rendre le classeur vers l’imprimante |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassWorkbookRenderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d’exemple et définir la taille de page
            worksheet.Cells["A1"].PutValue("Workbook Render Demo");
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Créer des options d’image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Créer le rendu du classeur et obtenir la taille de la page
            WorkbookRender render = new WorkbookRender(workbook, options);
            float[] pageSize = render.GetPageSizeInch(0);
            
            // Afficher les résultats
            Console.WriteLine($"Page Width: {pageSize[0]} inches");
            Console.WriteLine($"Page Height: {pageSize[1]} inches");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


