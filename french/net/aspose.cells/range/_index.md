---
title: Range
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule lobjet qui représente une plage de cellules dans une feuille de calcul.
type: docs
weight: 5030
url: /fr/net/aspose.cells/range/
---
## Range class

Encapsule l'objet qui représente une plage de cellules dans une feuille de calcul.

```csharp
public class Range
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | Obtient l'adresse de la plage. |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | Obtient le nombre de colonnes dans la plage. |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | Définit ou obtient la largeur de colonne de cette plage |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | Renvoie un objet Range qui représente la région actuelle. La région actuelle est une plage délimitée par n'importe quelle combinaison de lignes vides et de colonnes vides. |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | Obtient un objet Range qui représente la ou les colonnes entières contenant la plage spécifiée. |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | Obtient un objet Range qui représente la ligne entière (ou les lignes) contenant la plage spécifiée. |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | Obtient l'index de la première colonne de la plage. |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | Obtient l'index de la première ligne de la plage. |
| [Height](../../aspose.cells/range/height) { get; } | Obtient la largeur d'une plage en points. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | Obtient tous les liens hypertexte de la plage. |
| [Item](../../aspose.cells/range/item) { get; } | Obtient[`Cell`](../cell) objet dans cette plage. |
| [Left](../../aspose.cells/range/left) { get; } | Obtient la distance, en points, entre le bord gauche de la colonne A et le bord gauche de la plage. |
| [Name](../../aspose.cells/range/name) { get; set; } | Obtient ou définit le nom de la plage. |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | Obtient les références de la plage. |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | Obtient le nombre de lignes dans la plage. |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | Définit ou obtient la hauteur des lignes dans cette plage |
| [Top](../../aspose.cells/range/top) { get; } | Obtient la distance, en points, entre le bord supérieur de la ligne 1 et le bord supérieur de la plage. |
| [Value](../../aspose.cells/range/value) { get; set; } | Obtient et définit la valeur de la plage. |
| [Width](../../aspose.cells/range/width) { get; } | Obtient la largeur d'une plage en points. |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | Obtient le[`Worksheet`](./worksheet) objet qui contient cette plage. |

## Méthodes

| Nom | La description |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | Applique les formats pour toute une plage. |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | Remplir automatiquement la plage cible. |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | Remplir automatiquement la plage cible. |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | Copie les données (y compris les formules), la mise en forme, les objets de dessin, etc. à partir d'une plage source. |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | Copie de la plage avec options spéciales de collage. |
| [CopyData](../../aspose.cells/range/copydata)(Range) | Copie les données de cellule (y compris les formules) à partir d'une plage source. |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | Copie les paramètres de style d'une plage source. |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | Copie la valeur de la cellule à partir d'une plage source. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | Exporte les données de cette plage vers unDataTable objet. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | Exporte les données de cette plage vers unDataTable objet. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | Exporte les données de cette plage vers unDataTable objet. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | Obtient[`Cell`](../cell) objet ou null dans cette plage. |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | Obtient l'énumérateur pour les cellules de cette plage. |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | Obtient[`Range`](../range) plage par décalage. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | Renvoie un[`Range`](../range) objet qui représente l'intersection rectangulaire de deux plages. |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | Indique si la plage est intersectée. |
| [Merge](../../aspose.cells/range/merge)() | Combine une plage de cellules en une seule cellule. |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | Déplacer la plage actuelle vers la plage de destination. |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | Met une valeur dans la plage, le cas échéant, la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | Définir les bordures intérieures de la plage. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | Définit une bordure de contour autour d'une plage de cellules. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | Définit les bordures du contour autour d'une plage de cellules avec le même style et la même couleur de bordure. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | Définit des bordures de lignes autour d'une plage de cellules. |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | Définit le style de la plage. |
| override [ToString](../../aspose.cells/range/tostring)() | Renvoie une chaîne représentant l'objet Range actuel. |
| [Union](../../aspose.cells/range/union)(Range) | Renvoie l'union de deux plages. |
| [UnMerge](../../aspose.cells/range/unmerge)() | Défusionne les cellules fusionnées de cette plage. |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
// Récupère les premières cellules de la feuille de calcul.
Cells cells = workbook.Worksheets[0].Cells;
// Crée une plage (A1:D3).
Range range = cells.CreateRange("A1", "D3");
// Définissez la valeur sur la plage.
range.Value = "Hello";
// Enregistrer le fichier Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()
'Obtenez les premières cellules de feuille de calcul.
Dim cells as Cells = workbook.Worksheets[0].Cells
'Créez une plage (A1:D3).
Dim range as Range = cells.CreateRange("A1", "D3")
'Définissez la valeur sur la plage.
range.Value = "Hello"
'Enregistrez le fichier Excel
workbook.Save("book1.xlsm")
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
