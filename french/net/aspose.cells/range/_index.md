---
title: "Classe Range"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Range. Encapsule l'objet qui représente une plage de cellules dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/range/
---
## Range class

Encapsule l'objet qui représente une plage de cellules dans une feuille de calcul.

```csharp
public class Range : IEnumerable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Range](range/#constructor)(CellArea, Cells) | Constructeur de classe. |
| [Range](range/#constructor_1)(int, int, int, int, Cells) | Constructeur de classe. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Address](../../aspose.cells/range/address/) { get; } | Obtient l'adresse de la plage. |
| [ColumnCount](../../aspose.cells/range/columncount/) { get; } | Obtient le nombre de colonnes dans la plage. |
| [ColumnWidth](../../aspose.cells/range/columnwidth/) { get; set; } | Définit ou obtient la largeur de colonne de cette plage |
| [CurrentRegion](../../aspose.cells/range/currentregion/) { get; } | Renvoie un objet Range qui représente la région actuelle. La région actuelle est une plage délimitée par toute combinaison de lignes vides et de colonnes vides. |
| [EntireColumn](../../aspose.cells/range/entirecolumn/) { get; } | Obtient un objet Range qui représente la colonne entière (ou les colonnes) contenant la plage spécifiée. |
| [EntireRow](../../aspose.cells/range/entirerow/) { get; } | Obtient un objet Range qui représente la ligne entière (ou les lignes) contenant la plage spécifiée. |
| [FirstColumn](../../aspose.cells/range/firstcolumn/) { get; } | Obtient l'index de la première colonne de la plage. |
| [FirstRow](../../aspose.cells/range/firstrow/) { get; } | Obtient l'index de la première ligne de la plage. |
| [Height](../../aspose.cells/range/height/) { get; } | Obtient la largeur d'une plage en points. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks/) { get; } | Obtient tous les hyperliens dans la plage. |
| [Item](../../aspose.cells/range/item/) { get; } | Obtient l'objet [`Cell`](../cell/) dans cette plage. |
| [Left](../../aspose.cells/range/left/) { get; } | Obtient la distance, en points, du bord gauche de la colonne A au bord gauche de la plage. |
| [Name](../../aspose.cells/range/name/) { get; set; } | Obtient ou définit le nom de la plage. |
| [RefersTo](../../aspose.cells/range/refersto/) { get; } | Obtient la référence de la plage. |
| [RowCount](../../aspose.cells/range/rowcount/) { get; } | Obtient le nombre de lignes dans la plage. |
| [RowHeight](../../aspose.cells/range/rowheight/) { get; set; } | Définit ou obtient la hauteur des lignes dans cette plage |
| [Top](../../aspose.cells/range/top/) { get; } | Obtient la distance, en points, du bord supérieur de la ligne 1 au bord supérieur de la plage. |
| [Value](../../aspose.cells/range/value/) { get; set; } | Obtient et définit la valeur de la plage. |
| [Width](../../aspose.cells/range/width/) { get; } | Obtient la largeur d'une plage en points. |
| [Worksheet](../../aspose.cells/range/worksheet/) { get; } | Obtient l'objet [`Worksheet`](./worksheet/) qui contient cette plage. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddHyperlink](../../aspose.cells/range/addhyperlink/)(string, string, string) | Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules. |
| [ApplyStyle](../../aspose.cells/range/applystyle/)(Style, StyleFlag) | Applique des formats à une plage entière. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill)(Range) | Remplit automatiquement la plage cible. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill_1)(Range, AutoFillType) | Remplit automatiquement la plage cible. |
| [Clear](../../aspose.cells/range/clear/)() | Efface cette plage. |
| [ClearComments](../../aspose.cells/range/clearcomments/)() | Efface les commentaires de cette plage. |
| [ClearContents](../../aspose.cells/range/clearcontents/)() | Efface le contenu de cette plage. |
| [ClearFormats](../../aspose.cells/range/clearformats/)() | Efface les formats de cette plage. |
| [ClearHyperlinks](../../aspose.cells/range/clearhyperlinks/)(bool) | Supprime uniquement les hyperliens. |
| [Copy](../../aspose.cells/range/copy/#copy)(Range) | Copie les données (y compris les formules), le formatage, les objets de dessin, etc. depuis une plage source. |
| [Copy](../../aspose.cells/range/copy/#copy_1)(Range, PasteOptions) | Copie la plage avec les options de collage spécial. |
| [CopyData](../../aspose.cells/range/copydata/)(Range) | Copie les données de cellule (y compris les formules) depuis une plage source. |
| [CopyStyle](../../aspose.cells/range/copystyle/)(Range) | Copie les paramètres de style depuis une plage source. |
| [CopyValue](../../aspose.cells/range/copyvalue/)(Range) | Copie la valeur de cellule depuis une plage source. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable)() | Exporte les données de cette plage vers un objet DataTable. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable_1)(ExportTableOptions) | Exporte les données de cette plage vers un objet DataTable. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring/)() | Exporte les données de cette plage vers un objet DataTable. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull/)(int, int) | Obtient l'objet [`Cell`](../cell/) ou null dans cette plage. |
| [GetEnumerator](../../aspose.cells/range/getenumerator/)() | Obtient l'énumérateur des cellules de cette `Range`. |
| [GetOffset](../../aspose.cells/range/getoffset/)(int, int) | Obtient la plage `Range` par décalage. |
| [Intersect](../../aspose.cells/range/intersect/)(Range) | Renvoie un objet `Range` qui représente l'intersection rectangulaire de deux plages. |
| [IsBlank](../../aspose.cells/range/isblank/)() | Indique si la plage contient des valeurs. |
| [IsIntersect](../../aspose.cells/range/isintersect/)(Range) | Indique si la plage intersecte. |
| [Merge](../../aspose.cells/range/merge/)() | Combine une plage de cellules en une seule cellule. |
| [MoveTo](../../aspose.cells/range/moveto/)(int, int) | Déplace la plage actuelle vers la plage de destination. |
| [PutValue](../../aspose.cells/range/putvalue/)(string, bool, bool) | Insère une valeur dans la plage, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders/)(BorderType, CellBorderType, CellsColor) | Définit les bordures internes de la plage. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder)(BorderType, CellBorderType, CellsColor) | Définit la bordure extérieure autour d'une plage de cellules. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder_1)(BorderType, CellBorderType, Color) | Définit la bordure extérieure autour d'une plage de cellules. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_2)(CellBorderType[], Color[]) | Définit les bordures extérieures autour d'une plage de cellules. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle)(Style) | Définit le style de la plage. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle_1)(Style, bool) | Appliquer le style de cellule. |
| [ToHtml](../../aspose.cells/range/tohtml/)(HtmlSaveOptions) | Convertir la plage en html . |
| [ToImage](../../aspose.cells/range/toimage/)(ImageOrPrintOptions) | Convertit la plage en image. |
| [ToJson](../../aspose.cells/range/tojson/)(JsonSaveOptions) | Convertir la plage en valeur JSON. |
| override [ToString](../../aspose.cells/range/tostring/)() | Renvoie une chaîne représentant l’objet Range actuel. |
| [Transpose](../../aspose.cells/range/transpose/)() | Transposer (faire pivoter) les données des lignes aux colonnes ou inversement. |
| [Union](../../aspose.cells/range/union/)(Range) | (**Obsolète.**) Retourne l'union de deux plages. |
| [UnionRang](../../aspose.cells/range/unionrang/)(Range) | (**Obsolète.**) Retourne le résultat de l'union de deux plages. |
| [UnionRanges](../../aspose.cells/range/unionranges/)(Range[]) | Retourne le résultat de l'union de deux plages. |
| [UnMerge](../../aspose.cells/range/unmerge/)() | Démarque les cellules fusionnées de cette plage. |

### Remarques

La classe Range désigne une région d'une feuille de calcul Excel. Avec celle‑ci, vous pouvez formater et définir la valeur de la plage. Et vous pouvez également copier simplement une plage d'Excel aussi.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "D3");
            range.Value = "Hello";
            workbook.Save("book1.xlsm");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


