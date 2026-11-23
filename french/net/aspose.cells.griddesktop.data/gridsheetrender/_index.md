---
title: "Class GridSheetRender"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridDesktop.Data.GridSheetRender class. Représente un rendu de feuille de calcul qui peut rendre la feuille de calcul en diverses images telles que BMP, PNG, JPEG, TIFF.. Le constructeur de cette classe doit être utilisé après la modification du style de la cellule de la configuration de page"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridsheetrender/
---
## GridSheetRender class

Représente un rendu de feuille de calcul qui peut rendre la feuille de calcul en diverses images telles que (BMP, PNG, JPEG, TIFF...). Le constructeur de cette classe doit être utilisé après la modification de la configuration de page, du style de cellule.

```csharp
public class GridSheetRender
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [GridSheetRender](gridsheetrender/)(Worksheet, GridImageOrPrintOptions) | la construction de SheetRender, nécessite la feuille de calcul et ImageOrPrintOptions comme paramètres |

## Propriétés

| Nom | Description |
| --- | --- |
| [PageCount](../../aspose.cells.griddesktop.data/gridsheetrender/pagecount/) { get; } | Obtient le nombre total de pages de la feuille de calcul actuelle. |
| [PageScale](../../aspose.cells.griddesktop.data/gridsheetrender/pagescale/) { get; } | Obtient l'échelle de page calculée de la feuille. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetPageSizeInch](../../aspose.cells.griddesktop.data/gridsheetrender/getpagesizeinch/)(int) | Obtenir la taille de page en pouces de l’image de sortie. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage)(int) | Rendre une page donnée vers un objet Bitmap. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_3)(int, Stream) | Rendre une page donnée vers un flux. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_4)(int, string) | Rendre une page donnée vers un fichier. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Rendre une certaine page vers un Graphics |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Rendre une certaine page vers un Graphics |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter)(PrinterSettings) | Rendre la feuille de calcul vers l'imprimante |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_2)(string) | Rendre la feuille de calcul vers l'imprimante |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Rendre la feuille de calcul vers l'imprimante |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_3)(string, string) | Rendre la feuille de calcul vers l'imprimante |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff)(Stream) | Rendre toute la feuille de calcul en image Tiff vers le flux. |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff_1)(string) | Rendre toute la feuille de calcul en image Tiff vers un fichier. |

### Voir aussi

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


