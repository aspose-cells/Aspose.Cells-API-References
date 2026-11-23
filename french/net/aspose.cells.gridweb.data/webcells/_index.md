---
title: "Classe WebCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridWeb.Data.WebCells classe."
type: docs
url: /fr/net/aspose.cells.gridweb.data/webcells/
---
## WebCells class

```csharp
[Obsolete("This class is obsolete; use  GridCells instead")]
public class WebCells
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/webcells/count/) { get; } | Obtient le nombre de cellules. |
| [Item](../../aspose.cells.gridweb.data/webcells/item/) { get; } | Obtient l'élément Cell à l'index de ligne et de colonne de cellule spécifiés. (2 indexeurs) |
| [MaxColumn](../../aspose.cells.gridweb.data/webcells/maxcolumn/) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/webcells/maxrow/) { get; } |  |
| [MergedCells](../../aspose.cells.gridweb.data/webcells/mergedcells/) { get; } | Obtient la collection de cellules fusionnées. |
| [MinColumn](../../aspose.cells.gridweb.data/webcells/mincolumn/) { get; } | Numéro de colonne minimal de la cellule contenant des données ou un style. |
| [MinRow](../../aspose.cells.gridweb.data/webcells/minrow/) { get; } | Numéro de ligne minimal de la cellule contenant des données ou un style. |
| [StandardHeight](../../aspose.cells.gridweb.data/webcells/standardheight/) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en points. |
| [StandardWidth](../../aspose.cells.gridweb.data/webcells/standardwidth/) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en caractères. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/webcells/clear/)() |  |
| [ClearContents](../../aspose.cells.gridweb.data/webcells/clearcontents/)(int, int, int, int) | Efface le contenu d'une plage. |
| [DeleteColumn](../../aspose.cells.gridweb.data/webcells/deletecolumn/)(int) | Supprime une colonne. |
| [DeleteRow](../../aspose.cells.gridweb.data/webcells/deleterow/)(int) | Supprime une ligne. |
| [DeleteRows](../../aspose.cells.gridweb.data/webcells/deleterows/)(int, int) | Supprime un certain nombre de lignes. Cette méthode est beaucoup plus rapide que DeleteRow lors d'une suppression de lignes en lot. |
| [Export](../../aspose.cells.gridweb.data/webcells/export/)(int, int, int, int, bool, bool) | Exporte les données de la collection Cells d'un WebWorksheet vers un nouvel objet DataTable |
| [ExportArray](../../aspose.cells.gridweb.data/webcells/exportarray/)(int, int, int, int) | Exporte les données de la collection Cells vers un objet tableau à deux dimensions. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/webcells/getcolumncaption/)(int) | Obtient la légende de la colonne. Si la légende n'est pas définie, renvoie une chaîne vide. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/webcells/getcolumnreadonly/)(int) | Obtient si une colonne est en lecture seule. il s'agit d'une méthode étendue de GridWeb spécifiquement, elle ne sera pas conservée ni prise en compte dans le fichier Excel réel. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/webcells/getcolumnwidth/)(int) | Obtient la largeur de la colonne spécifiée |
| [GetEnumerator](../../aspose.cells.gridweb.data/webcells/getenumerator/)() | Obtient l'énumérateur des cellules |
| [GetRowCaption](../../aspose.cells.gridweb.data/webcells/getrowcaption/)(int) | Obtient la légende de la ligne. Si la légende n'est pas définie, renvoie une chaîne vide. |
| [GetRowHeight](../../aspose.cells.gridweb.data/webcells/getrowheight/)(int) | Obtient la hauteur d'une ligne spécifiée. |
| [GetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/getrowhiddenstatus/)(int) | Obtient le statut masqué d'une ligne spécifiée. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/getrowoutlinelevel/)(int) | Obtient le niveau de contour de la ligne. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/webcells/getrowreadonly/)(int) | Obtient si une ligne est en lecture seule. Cette méthode étendue de GridWeb spécifiquement ne sera pas conservée et n'affectera pas le fichier Excel réel. |
| [InsertColumn](../../aspose.cells.gridweb.data/webcells/insertcolumn/)(int) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertRow](../../aspose.cells.gridweb.data/webcells/insertrow/)(int) | Insère une nouvelle ligne dans la feuille de calcul. |
| [InsertRows](../../aspose.cells.gridweb.data/webcells/insertrows/)(int, int) | Insère plusieurs lignes dans la feuille de calcul. |
| [Merge](../../aspose.cells.gridweb.data/webcells/merge/)(int, int, int, int) |  |
| [SetBorders](../../aspose.cells.gridweb.data/webcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Définit les bordures d'une plage de cellules. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/webcells/setcolumncaption/)(int, string) | Définit la légende pour la colonne. Veuillez noter que c'est un attribut d'extension et qu'il ne peut pas être conservé dans le fichier Excel. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/webcells/setcolumnreadonly/)(int, bool) | Définit une colonne en lecture seule afin que l'utilisateur ne puisse pas la supprimer côté client. Cette méthode étendue de GridWeb spécifiquement ne sera pas conservée et n'affectera pas le fichier Excel réel. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/webcells/setcolumnwidth/)(int, Unit) | Définit la largeur de la colonne spécifiée. Le type de largeur accepté est Point, Pixel ou Pouce. |
| [SetRowCaption](../../aspose.cells.gridweb.data/webcells/setrowcaption/)(int, string) | Définit la légende pour la ligne. |
| [SetRowHeight](../../aspose.cells.gridweb.data/webcells/setrowheight/)(int, Unit) | Définit la hauteur de la ligne spécifiée. Le type de largeur accepté est Point, Pixel ou Pouce. |
| [SetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/setrowhiddenstatus/)(int, bool) | Définit le statut masqué d'une ligne spécifiée. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevel/)(int, int) | Définit le niveau de contour de la ligne. |
| [SetRowOutlineLevelAndStatus](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevelandstatus/)(int, int, bool) | Définit le niveau de contour de la ligne. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/webcells/setrowreadonly/)(int, bool) | Définit une ligne en lecture seule afin que l'utilisateur ne puisse pas la supprimer côté client. Cette méthode étendue de GridWeb spécifiquement ne sera pas conservée et n'affectera pas le fichier Excel réel. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle_1)(string, TableItemStyle) | Applique le style à une plage de cellules spécifiée. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle)(int, int, int, int, TableItemStyle) | Applique le style à une plage de cellules spécifiée. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort)(int, int, int, int, int) | Trie les données en ordre ascendant de haut en bas dans une plage d'un WebWorksheet selon l'index de colonne spécifié. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_2)(int, int, int, int, int[]) | Trie les données en ordre ascendant de haut en bas dans une plage d'un WebWorksheet selon certains champs spécifiés par un tableau d'index de colonnes. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_1)(int, int, int, int, int, SortByOrder, SortOrientation, bool) | Trie les données en ordre ascendant de haut en bas dans une plage d'un WebWorksheet selon l'index de colonne spécifié. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_3)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Trie les données en ordre ascendant dans une plage d'un WebWorksheet selon certains champs spécifiés par un tableau d'index. |
| [UnMerge](../../aspose.cells.gridweb.data/webcells/unmerge/)(int, int, int, int) | Démarque une plage spécifiée de cellules fusionnées. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/webcells/cellindextoname/)(int, int) | Obtient le nom de la cellule selon ses indices de ligne et de colonne. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/webcells/cellnametoindex/)(string, out int, out int) | Obtient les indices de ligne et de colonne de la cellule selon son nom |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/webcells/columnindextoname/)(int) | Obtient le nom de la colonne selon l'indice de colonne. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/webcells/columnnametoindex/)(string) | Obtient l'indice de colonne selon le nom de la colonne. |

### Remarques

NOTE : Cette classe est maintenant obsolète. Veuillez utiliser GridCells à la place. Cette classe sera supprimée après 6 mois à compter d'août 2014. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


