---
title: "Classe GridCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridCells. Encapsule une collection d'objets GridCell"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

Encapsule une collection d'objets [`GridCell`](../gridcell/).

```csharp
public class GridCells : IEnumerable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns/) { get; } | Obtient la collection d'objets [`GridColumn`](../gridcolumn/) qui représente les colonnes individuelles de cette feuille de calcul. |
| [Count](../../aspose.cells.gridweb.data/gridcells/count/) { get; } | Obtient le nombre de cellules. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell/) { get; } | Obtient la première cellule de cette feuille de calcul. |
| [Item](../../aspose.cells.gridweb.data/gridcells/item/) { get; } | Obtient l'élément [`GridCell`](../gridcell/) à l'index de ligne et de colonne de cellule spécifié. (2 indexeurs) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell/) { get; } | Obtient la dernière cellule de cette feuille de calcul. |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn/) { get; } | Indice de colonne maximal de la cellule contenant des données ou un style. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn/) { get; } | Indice de colonne maximal de la cellule contenant des données. |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow/) { get; } | Indice de ligne maximal de la cellule contenant des données. |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow/) { get; } | Indice de ligne maximal de la cellule contenant des données ou un style. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells/) { get; } | Obtient la collection de cellules fusionnées. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn/) { get; } | Indice de colonne minimal des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée). |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn/) { get; } | Indice de colonne minimal de la cellule contenant des données. |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow/) { get; } | Indice de ligne minimal de la cellule contenant des données. |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow/) { get; } | Indice de ligne minimal de la cellule contenant des données ou un style. |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator/) { get; } | Obtient l'énumérateur des lignes |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows/) { get; } | Obtient la collection d'objets [`GridRow`](../gridrow/) qui représente les lignes individuelles de cette feuille de calcul. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight/) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en points. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels/) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth/) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en caractères. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch/) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pouces. |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels/) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pixels. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CheckCell](../../aspose.cells.gridweb.data/gridcells/checkcell/)(int, int) | Obtient l'élément [`GridCell`](../gridcell/) ou null à l'index de ligne et de colonne de cellule spécifié. |
| [CheckColumn](../../aspose.cells.gridweb.data/gridcells/checkcolumn/)(int) | Obtient l'élément [`GridColumn`](../gridcolumn/) ou null à l'index de colonne spécifié. |
| [CheckRow](../../aspose.cells.gridweb.data/gridcells/checkrow/)(int) | Obtient l'élément [`GridRow`](../gridrow/) ou null à l'index de ligne de cellule spécifié. |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear/)() | Efface toutes les cellules de la collection. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Efface le contenu d'une plage. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Efface le contenu d'une plage. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats)(GridCellArea) | Efface le formatage d'une plage. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Efface le formatage d'une plage. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange)(GridCellArea) | Efface le contenu et le formatage d'une plage. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Efface le contenu et le formatage d'une plage. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn/)(GridCells, int, int) | Copie les données et le formatage d'une colonne entière. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns/)(GridCells, int, int, int) | Copie les données et le formatage d'une colonne entière. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow/)(GridCells, int, int) | Copie les données et le formatage d'une ligne entière. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows/)(GridCells, int, int, int) | Copie les données et le formatage de plusieurs lignes entières. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns/)() | Supprime toutes les colonnes vides qui ne contiennent aucune donnée. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows/)() | Supprime toutes les lignes vides qui ne contiennent aucune donnée. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn)(int) | Supprime une colonne. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Supprime une colonne. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns/)(int, int, bool) | Supprime plusieurs colonnes. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange/)(int, int, int, int, GridShiftType) | Supprime une plage de cellules et décale les cellules selon l'option de décalage. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow/)(int) | Supprime une ligne. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows)(int, int) | Supprime plusieurs lignes. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Supprime plusieurs lignes dans la feuille de calcul. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export/)(int, int, int, int, bool, bool) | Exporte les données de la collection Cells d'un WebWorksheet vers un nouvel objet DataTable |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray/)(int, int, int, int) | Exporte les données de la collection `GridCells` vers un objet tableau à deux dimensions. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell/)(int, int) | Obtient l'élément [`GridCell`](../gridcell/) à l'index de ligne et de colonne de cellule spécifié. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth/)(int) | Obtient la largeur de la colonne spécifiée |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch/)(int) | Obtient la largeur de la colonne spécifiée, en pouces. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel/)(int) | Obtient la largeur de la colonne spécifiée, en pixels. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator/)() | Obtient l'énumérateur des lignes |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow/)(int) | Obtient l'élément [`GridRow`](../gridrow/) ou à l'index de ligne de cellule spécifié. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight/)(int) | Obtient la hauteur d'une ligne spécifiée. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch/)(int) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel/)(int) | Obtient la hauteur d'une ligne spécifiée en unité de pixel. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel/)(int) | Obtient le niveau de contour de la ligne. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel/)(int) | Obtenez la largeur dans différents types de vue. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Regroupe les colonnes. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Regroupe les colonnes. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows/)(int, int) | Regroupe les lignes. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn/)(int) | Masque une colonne. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow/)(int) | Masque une ligne. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn)(int) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Insère plusieurs colonnes dans la feuille de calcul. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Insère plusieurs colonnes dans la feuille de calcul. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange)(GridCellArea, GridShiftType) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange_1)(GridCellArea, int, GridShiftType, bool) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow/)(int) | Insère une nouvelle ligne dans la feuille de calcul. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows)(int, int) | Insère plusieurs lignes dans la feuille de calcul. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Insère plusieurs lignes dans la feuille de calcul. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn/)(int) | Vérifie si la colonne donnée est vide (ne contient aucune donnée). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden/)(int) | Vérifie si une colonne à l'index donné est masquée. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden/)(int) | Vérifie si une ligne à l'index donné est masquée. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge/)(int, int, int, int) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange/)(GridCellArea, int, int) | Déplace la plage. |
| [RemoveDuplicates](../../aspose.cells.gridweb.data/gridcells/removeduplicates/)(int, int, int, int) | Supprime les valeurs dupliquées dans la plage. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas/)() | Supprime toutes les formules et les remplace par la valeur de la formule. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Définit les bordures d'une plage de cellules. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth/)(int, double) | Définit la largeur de la colonne spécifiée. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch/)(int, double) | Définit la largeur de la colonne en pouces. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel/)(int, int) | Définit la largeur de la colonne en pixels. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight/)(int, double) | Définit la hauteur de la ligne spécifiée. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch/)(int, double) | Définit la hauteur de la ligne en pouces. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel/)(int, int) | Définit la hauteur de la ligne en unités de pixels. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel/)(int, int) | Définit le niveau de contour de la ligne. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle_1)(string, GridTableItemStyle) | Applique le style à une plage de cellules spécifiée. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle)(int, int, int, int, GridTableItemStyle) | Applique le style à une plage de cellules spécifiée. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Trie les données de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. Trie les données de gauche à droite dans une plage d'une feuille de calcul selon l'index de ligne spécifié. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Trie les données de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. Trie les données de gauche à droite dans une plage d'une feuille de calcul selon l'index de ligne spécifié. |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns/)(int, int) | Dégroupe les colonnes. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows/)(int, int) | Dégroupe les lignes. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn/)(int, double) | Dévoile une colonne |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow/)(int) | Dévoile une ligne. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge/)(int, int, int, int) | Démarque une plage spécifiée de cellules fusionnées. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname/)(int, int) | Obtient le nom de la cellule selon ses indices de ligne et de colonne. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex/)(string, out int, out int) | Obtient les indices de ligne et de colonne de la cellule selon son nom |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname/)(int) | Obtient le nom de la colonne selon l'indice de colonne. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex/)(string) | Obtient l'indice de colonne selon le nom de la colonne. |

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


