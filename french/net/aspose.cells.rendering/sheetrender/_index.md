---
title: "Classe SheetRender"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Rendering.SheetRender. Représente un rendu de feuille de calcul qui peut rendre la feuille de calcul en diverses images telles que BMP, PNG, JPEG, TIFF.. Le constructeur de cette classe doit être utilisé après la modification du style de cellule de la configuration de page."
type: docs
url: /fr/net/aspose.cells.rendering/sheetrender/
---
## SheetRender class

Représente un rendu de feuille de calcul qui peut rendre la feuille de calcul en diverses images telles que (BMP, PNG, JPEG, TIFF...). Le constructeur de cette classe doit être utilisé après la modification de la configuration de page, du style de cellule.

```csharp
public class SheetRender
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SheetRender](sheetrender/)(Worksheet, ImageOrPrintOptions) | la construction de SheetRender, nécessite la feuille de calcul et ImageOrPrintOptions comme paramètres |

## Propriétés

| Nom | Description |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/sheetrender/pagecount/) { get; } | Obtient le nombre total de pages de la feuille de calcul actuelle. |
| [PageScale](../../aspose.cells.rendering/sheetrender/pagescale/) { get; } | Obtient l'échelle de page calculée de la feuille. Retourne l'échelle définie si [`Zoom`](../../aspose.cells/pagesetup/zoom/) est définie. Sinon, retourne l'échelle calculée selon [`FitToPagesWide`](../../aspose.cells/pagesetup/fittopageswide/) et [`FitToPagesTall`](../../aspose.cells/pagesetup/fittopagestall/). |

## Méthodes

| Nom | Description |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/sheetrender/customprint/)(bool, PrintPageEventArgs) | Le client peut contrôler les paramètres de page de l’imprimante lors de l’impression de chaque page à l’aide de cette fonction. |
| [Dispose](../../aspose.cells.rendering/sheetrender/dispose/)() | Libère les ressources créées et utilisées pour le rendu. |
| [GetPageSizeInch](../../aspose.cells.rendering/sheetrender/getpagesizeinch/)(int) | Obtenir la taille de page en pouces de l’image de sortie. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage)(int) | Rendre une page donnée vers un objet Bitmap. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_3)(int, Stream) | Rendre une page donnée vers un flux. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_4)(int, string) | Rendre une page donnée vers un fichier. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Rendre une certaine page vers un Graphics |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Rendre une certaine page vers un Graphics |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter)(PrinterSettings) | Rendre la feuille de calcul vers l'imprimante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_2)(string) | Rendre la feuille de calcul vers l'imprimante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Rendre la feuille de calcul vers l'imprimante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_4)(string, string) | Rendre la feuille de calcul vers l'imprimante |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolète.**) Rendre la feuille de calcul vers l'imprimante |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff)(Stream) | Rendre toute la feuille de calcul en image Tiff vers le flux. |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff_1)(string) | Rendre toute la feuille de calcul en image Tiff vers un fichier. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassSheetRenderDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Configurer la mise en page
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.PrintArea = "1:10";
            pageSetup.SetFitToPages(1, 1);

            // Créer SheetRender et démontrer la fonctionnalité principale
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender sr = new SheetRender(sheet, options);
            
            Console.WriteLine($"Number of pages: {sr.PageCount}");
            Console.WriteLine($"Page scale: {sr.PageScale * 100}%");
            
            // Rendre la première page en image (démonstration)
            sr.ToImage(0, "output_page1.png");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


