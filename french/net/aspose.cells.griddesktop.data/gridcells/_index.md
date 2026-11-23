---
title: "Classe GridCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridDesktop.Data.GridCells. Encapsule une collection d'objets Cell"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Encapsule une collection d'objets Cell.

```csharp
public class GridCells : IEnumerable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns/) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count/) { get; } | Obtient le nombre de cellules. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell/) { get; } | Obtient la première cellule de cette feuille de calcul. |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item/) { get; } | Obtient l'élément [`GridCell`](../gridcell/) à l'index de ligne et de colonne de cellule spécifié. (2 indexeurs) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell/) { get; } | Obtient la dernière cellule de cette feuille de calcul. |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn/) { get; } | Indice de colonne maximal de la cellule contenant des données ou un style. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn/) { get; } | Indice de colonne maximal de la cellule contenant des données. |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow/) { get; } | Indice de ligne maximal de la cellule contenant des données. |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow/) { get; } | Indice de ligne maximal de la cellule contenant des données ou un style. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells/) { get; } | Obtient la collection de cellules fusionnées. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn/) { get; } | Indice de colonne minimal des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée). |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn/) { get; } | Indice de colonne minimal de la cellule contenant des données. |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow/) { get; } | Indice de ligne minimal de la cellule contenant des données. |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow/) { get; } | Indice de ligne minimal de la cellule contenant des données ou un style. |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator/) { get; } | Obtient l'énumérateur des lignes |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows/) { get; } | Obtient la collection d'objets [`GridRow`](../gridrow/) qui représente les lignes individuelles de cette feuille de calcul. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight/) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en points. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels/) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth/) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en caractères. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch/) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell/)(int, int) | Obtient l'élément [`GridCell`](../gridcell/) ou null à l'index de ligne et de colonne de cellule spécifié. |
| [CheckRow](../../aspose.cells.griddesktop.data/gridcells/checkrow/)(int) | Obtient l'élément [`GridRow`](../gridrow/) ou null à l'index de ligne de cellule spécifié. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear/)() | Efface toutes les cellules de la collection. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Efface le contenu d'une plage. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Efface le contenu d'une plage. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats)(GridCellArea) | Efface le formatage d'une plage. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Efface le formatage d'une plage. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange)(GridCellArea) | Efface le contenu et le formatage d'une plage. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Efface le contenu et le formatage d'une plage. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn/)(GridCells, int, int) | Copie les données et le formatage d'une colonne entière. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns/)(GridCells, int, int, int) | Copie les données et le formatage d'une colonne entière. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow/)(GridCells, int, int) | Copie les données et le formatage d'une ligne entière. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows/)(GridCells, int, int, int) | Copie les données et le formatage de plusieurs lignes entières. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns/)() | Supprime toutes les colonnes vides qui ne contiennent aucune donnée. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows/)() | Supprime toutes les lignes vides qui ne contiennent aucune donnée. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn)(int) | Supprime une colonne. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Supprime une colonne. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns/)(int, int, bool) | Supprime plusieurs colonnes. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow/)(int) | Supprime une ligne. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows)(int, int) | Supprime plusieurs lignes. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Supprime plusieurs lignes dans la feuille de calcul. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle/)(int, int) | Obtient le style de la cellule donnée. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn/)(int) | Obtient l'élément [`GridColumn`](../gridcolumn/) ou à l'index de colonne de cellule spécifié. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth/)(int) | Obtient la largeur de la colonne spécifiée |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch/)(int) | Obtient la largeur de la colonne spécifiée, en pouces. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel/)(int) | Obtient la largeur de la colonne spécifiée, en pixels. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator/)() | Obtient l'énumérateur des lignes |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow/)(int) | Obtient l'élément [`GridRow`](../gridrow/) ou à l'index de ligne de cellule spécifié. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight/)(int) | Obtient la hauteur d'une ligne spécifiée. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch/)(int) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel/)(int) | Obtient la hauteur d'une ligne spécifiée en unité de pixel. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel/)(int) | Obtenez la largeur dans différents types de vue. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Regroupe les colonnes. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Regroupe les colonnes. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows/)(int, int) | Regroupe les lignes. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn/)(int) | Masque une colonne. |
| [HideColumns](../../aspose.cells.griddesktop.data/gridcells/hidecolumns/)(int, int) | Masque plusieurs colonnes. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow/)(int) | Masque une ligne. |
| [HideRows](../../aspose.cells.griddesktop.data/gridcells/hiderows/)(int, int) | Masque plusieurs lignes. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn)(int) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Insère plusieurs colonnes dans la feuille de calcul. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Insère plusieurs colonnes dans la feuille de calcul. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow/)(int) | Insère une nouvelle ligne dans la feuille de calcul. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows)(int, int) | Insère plusieurs lignes dans la feuille de calcul. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Insère plusieurs lignes dans la feuille de calcul. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn/)(int) | Vérifie si la colonne donnée est vide (ne contient aucune donnée). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden/)(int) | Vérifie si une colonne à l'index donné est masquée. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden/)(int) | Vérifie si une ligne à l'index donné est masquée. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge/)(int, int, int, int) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas/)() | Supprime toutes les formules et les remplace par la valeur de la formule. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth/)(int, double) | Définit la largeur de la colonne spécifiée. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch/)(int, double) | Définit la largeur de la colonne en pouces. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel/)(int, int) | Définit la largeur de la colonne en pixels. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight/)(int, double) | Définit la hauteur de la ligne spécifiée. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch/)(int, double) | Définit la hauteur de la ligne en pouces. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel/)(int, int) | Définit la hauteur de la ligne en unités de pixels. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle)(CellRange, Style) | Applique le style à une plage de cellules spécifiée. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_2)(string, Style) | Applique le style à une plage de cellules spécifiée. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_1)(int, int, int, int, Style) | Applique le style à une plage de cellules spécifiée. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Trie les données de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. Trie les données de gauche à droite dans une plage d'une feuille de calcul selon l'index de ligne spécifié. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) | Trie les données de la zone. |
| [SortAsNumber](../../aspose.cells.griddesktop.data/gridcells/sortasnumber/)(int, int, int, int, int[], SortOrder[], SortOrientation) | Trie les données de la zone (les données de la colonne clé doivent être numériques). |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns/)(int, int) | Dégroupe les colonnes. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows/)(int, int) | Dégroupe les lignes. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn/)(int, double) | Dévoile une colonne |
| [UnhideColumns](../../aspose.cells.griddesktop.data/gridcells/unhidecolumns/)(int, int, double) | Dévoile plusieurs colonnes. |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow/)(int, int) | Dévoile une ligne. |
| [UnhideRows](../../aspose.cells.griddesktop.data/gridcells/unhiderows/)(int, int, double) | Dévoile les lignes cachées. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge/)(int, int, int, int) | Démarque une plage spécifiée de cellules fusionnées. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname/)(int, int) | Obtient le nom de la cellule selon ses indices de ligne et de colonne. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex/)(string, out int, out int) | Obtient les indices de ligne et de colonne de la cellule selon son nom |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname/)(int) | Obtient le nom de la colonne selon l'indice de colonne. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex/)(string) | Obtient l'indice de colonne selon le nom de la colonne. |

### Voir aussi

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


