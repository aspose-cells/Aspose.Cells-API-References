---
title: "Classe Cells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Cells. Encapsule une collection d'objets pertinents aux cellules tels que Cell Row ...etc"
type: docs
url: /fr/net/aspose.cells/cells/
---
## Cells class

Encapsule une collection d'objets pertinents aux cellules, tels que [`Cell`](../cell/), [`Row`](../row/), ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns/) { get; } | Obtient la collection d'objets [`Column`](../column/) qui représente les colonnes individuelles de cette feuille de calcul. |
| [Count](../../aspose.cells/cells/count/) { get; } | Obtient le nombre total d'objets Cell instanciés. |
| [CountLarge](../../aspose.cells/cells/countlarge/) { get; } | Obtient le nombre total d'objets Cell instanciés. |
| [FirstCell](../../aspose.cells/cells/firstcell/) { get; } | Obtient la première cellule de cette feuille de calcul. |
| [IsDefaultColumnHidden](../../aspose.cells/cells/isdefaultcolumnhidden/) { get; set; } |  |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched/) { get; set; } | Indique que la hauteur de ligne et la hauteur de police par défaut correspondent. |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden/) { get; set; } | Indique si la ligne est masquée par défaut. |
| [Item](../../aspose.cells/cells/item/) { get; } | Obtient l'élément [`Cell`](../cell/) à l'index de ligne de cellule et à l'index de colonne spécifiés. (2 indexeurs) |
| [LastCell](../../aspose.cells/cells/lastcell/) { get; } | Obtient la dernière cellule de cette feuille de calcul. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn/) { get; } | Indice de colonne maximal des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn/) { get; } | Indice de colonne maximal de la cellule contenant des données. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow/) { get; } | Indice de ligne maximal de la cellule contenant des données. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange/) { get; } | Obtient la plage maximale qui inclut les données, les cellules fusionnées et les formes. |
| [MaxRow](../../aspose.cells/cells/maxrow/) { get; } | Indice de ligne maximal de la cellule contenant des données ou un style. |
| [MemorySetting](../../aspose.cells/cells/memorysetting/) { get; set; } | Obtient ou définit l'option d'utilisation de la mémoire pour ces cellules. |
| [MergedCells](../../aspose.cells/cells/mergedcells/) { get; } | (**Obsolete.**) Obtient la collection de cellules fusionnées. |
| [MinColumn](../../aspose.cells/cells/mincolumn/) { get; } | Indice de colonne minimal des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn/) { get; } | Indice de colonne minimal de la cellule contenant des données. |
| [MinDataRow](../../aspose.cells/cells/mindatarow/) { get; } | Indice de ligne minimal de la cellule contenant des données. |
| [MinRow](../../aspose.cells/cells/minrow/) { get; } | Indice de ligne minimal de la cellule contenant des données ou un style. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading/) { get; set; } | Obtient ou définit si le modèle de données des cellules doit prendre en charge la lecture Multi-Thread. La valeur par défaut de cette propriété est false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields/) { get; } | Obtient la liste des champs d'ods. |
| [PreserveString](../../aspose.cells/cells/preservestring/) { get; set; } | Obtient ou définit une valeur indiquant si toutes les valeurs de la feuille de calcul sont conservées sous forme de chaînes. La valeur par défaut est false. |
| [Ranges](../../aspose.cells/cells/ranges/) { get; } | Obtient la collection d'objets [`Range`](../range/) créés à l'exécution. |
| [Rows](../../aspose.cells/cells/rows/) { get; } | Obtient la collection d'objets [`Row`](../row/) qui représente les lignes individuelles de cette feuille de calcul. |
| [StandardHeight](../../aspose.cells/cells/standardheight/) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en points. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch/) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pouces. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels/) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels. |
| [StandardWidth](../../aspose.cells/cells/standardwidth/) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en caractères. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch/) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pouces. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels/) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pixels. |
| [Style](../../aspose.cells/cells/style/) { get; set; } | Obtient et définit le style par défaut de la feuille de calcul. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange/)(Range) | Ajoute une référence d'objet de plage aux cellules |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle/)(int, Style, StyleFlag) | Applique des formats à une colonne entière. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle/)(int, Style, StyleFlag) | Applique les formats à toute la ligne. |
| [ApplyStyle](../../aspose.cells/cells/applystyle/)(Style, StyleFlag) | Applique des formats à une feuille de calcul entière. |
| [CheckCell](../../aspose.cells/cells/checkcell/)(int, int) | Obtient l'élément [`Cell`](../cell/) ou null à l'indice de ligne et de colonne de cellule spécifié. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn/)(int) | Obtient l'élément [`Column`](../column/) ou null à l'indice de colonne spécifié. |
| [CheckRow](../../aspose.cells/cells/checkrow/)(int) | Obtient l'élément [`Row`](../row/) ou null à l'indice de ligne de cellule spécifié. |
| [Clear](../../aspose.cells/cells/clear/)() | Efface toutes les données de la feuille de calcul. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents)(CellArea) | Efface le contenu d'une plage. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents_1)(int, int, int, int) | Efface le contenu d'une plage. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats)(CellArea) | Efface le formatage d'une plage. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats_1)(int, int, int, int) | Efface le formatage d'une plage. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells/)() | Efface toutes les plages fusionnées. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange)(CellArea) | Efface le contenu et le formatage d'une plage. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange_1)(int, int, int, int) | Efface le contenu et le formatage d'une plage. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue/)() | Convertit toutes les données de type chaîne dans la feuille de calcul en valeur numérique si possible. |
| [CopyColumn](../../aspose.cells/cells/copycolumn/)(Cells, int, int) | Copie les données et les formats d'une colonne entière. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns)(Cells, int, int, int) | Copie les données et les formats de colonnes entières. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_2)(Cells, int, int, int, int) | Copie les données et les formats de toutes les colonnes. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_1)(Cells, int, int, int, PasteOptions) | Copie les données et les formats d'une colonne entière. |
| [CopyRow](../../aspose.cells/cells/copyrow/)(Cells, int, int) | Copie les données et les formats d'une ligne entière. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows)(Cells, int, int, int) | Copie les données et les formats de certaines lignes entières. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_1)(Cells, int, int, int, CopyOptions) | Copie les données et les formats de certaines lignes entières. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Copie les données et les formats de certaines lignes entières. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_2)(string) | Crée un objet [`Range`](../range/) à partir d'une adresse de la plage. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_3)(string, string) | Crée un objet [`Range`](../range/) à partir d'une plage de cellules. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange)(int, int, bool) | Crée un objet [`Range`](../range/) à partir de lignes de cellules ou de colonnes de cellules. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_1)(int, int, int, int) | Crée un objet [`Range`](../range/) à partir d'une plage de cellules. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns)() | Supprime toutes les colonnes vides qui ne contiennent aucune donnée. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns_1)(DeleteOptions) | Supprime toutes les colonnes vides qui ne contiennent aucune donnée. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows)() | Supprime toutes les lignes vides qui ne contiennent aucune donnée ou autre objet. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows_1)(DeleteOptions) | Supprime toutes les lignes vides qui ne contiennent aucune donnée ou certains objets spéciaux tels que les commentaires visibles, les tableaux croisés dynamiques. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn)(int) | Supprime une colonne. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn_1)(int, bool) | Supprime une colonne. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns_1)(int, int, bool) | Supprime plusieurs colonnes. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns)(int, int, DeleteOptions) | Supprime plusieurs colonnes. |
| [DeleteRange](../../aspose.cells/cells/deleterange/)(int, int, int, int, ShiftType) | Supprime une plage de cellules et décale les cellules selon l'option de décalage. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow)(int) | Supprime une ligne. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow_1)(int, bool) | Supprime une ligne. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows)(int, int) | Supprime plusieurs lignes. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_2)(int, int, bool) | Supprime plusieurs lignes dans la feuille de calcul. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_1)(int, int, DeleteOptions) | Supprime plusieurs lignes dans la feuille de calcul. |
| [Dispose](../../aspose.cells/cells/dispose/)() | Effectue des tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn)(int) | Obtient la dernière cellule de cette colonne. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn_1)(int, int, int, int) | Obtient la dernière cellule avec l'indice de colonne maximal dans cette plage. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow)(int) | Obtient la dernière cellule de cette ligne. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow_1)(int, int, int, int) | Obtient la dernière cellule avec l'indice de ligne maximal dans cette plage. |
| [ExportArray](../../aspose.cells/cells/exportarray/)(int, int, int, int) | Exporte les données de la collection `Cells` vers un objet tableau à deux dimensions. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable)(int, int, int, int) | Exporte les données de la collection `Cells` vers un objet DataTable. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_2)(int, int, int, int, bool) | Exporte les données de la collection `Cells` vers un objet DataTable. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Exporte les données de la collection `Cells` vers un objet DataTable. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring)(int, int, int, int) | Exporte les données de la collection `Cells` vers un objet DataTable. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring_1)(int, int, int, int, bool) | Exporte les données de la collection `Cells` vers un objet DataTable. |
| [ExportList&lt;T&gt;](../../aspose.cells/cells/exportlist/)(int, int, int, int, ExportTableOptions) |  |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray/)(int, int, int, int) | Exporte le type de valeur des cellules de la collection `Cells` vers un objet tableau à deux dimensions. |
| [Find](../../aspose.cells/cells/find/#find)(object, Cell) | Trouve la cellule contenant l'objet d'entrée. |
| [Find](../../aspose.cells/cells/find/#find_1)(object, Cell, FindOptions) | Trouve la cellule contenant l'objet d'entrée. |
| [GetCell](../../aspose.cells/cells/getcell/)(int, int) | (**Obsolete.**) Obtient l'élément [`Cell`](../cell/) ou null à l'index de ligne de cellule et d'index de colonne spécifiés. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle)(int, int) | Obtient le style d'affichage de la cellule donnée. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle_1)(int, int, BorderType) | Obtient le style d'affichage de la cellule donnée. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle/)(int, int) | Obtient le style de la cellule donnée. |
| [GetCellsWithPlaceInCellPicture](../../aspose.cells/cells/getcellswithplaceincellpicture/)() | Obtient toutes les cellules qui contiennent une image intégrée. |
| [GetColumnOriginalWidthPoint](../../aspose.cells/cells/getcolumnoriginalwidthpoint/)(int) | (**Obsolete.**) Obtient la hauteur d'origine de la colonne en points si la colonne est masquée |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth)(int) | Obtient la largeur (en unités de caractères) de la colonne spécifiée en vue normale |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth_1)(int, bool, CellsUnitType) | Obtient la largeur de la colonne. |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch/)(int) | (**Obsolete.**) Obtient la largeur de la colonne spécifiée en vue normale, en unités de pouces. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel)(int) | Obtient la largeur de la colonne spécifiée en vue normale, en unités de pixels. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel_1)(int, bool) | (**Obsolete.**) Obtient la largeur de la colonne spécifiée en vue normale, en unités de pixels. |
| [GetDependents](../../aspose.cells/cells/getdependents/)(bool, int, int) | Obtient toutes les cellules qui font référence à la cellule spécifique. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation/)(int, int, bool) | Obtient toutes les cellules dont le résultat calculé dépend de la cellule spécifique. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator/)() | Obtient l'énumérateur des cellules. |
| [GetFirstDataRow](../../aspose.cells/cells/getfirstdatarow/)(int) | Obtient l'index de la première ligne de la cellule qui contient des données dans la colonne spécifiée. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel/)(int) | Obtient le niveau de contour (à base zéro) de la colonne. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel/)(int) | Obtient le niveau de contour (à base zéro) de la ligne. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow/)(int) | Obtient l'index de la dernière ligne de la cellule qui contient des données dans la colonne spécifiée. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/)() | Obtient le niveau de contour maximal des colonnes groupées (à base zéro). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel/)() | Obtient le niveau de contour maximal des lignes groupées (à base zéro). |
| [GetMergedAreas](../../aspose.cells/cells/getmergedareas/)() | Obtient toutes les cellules fusionnées. |
| [GetRow](../../aspose.cells/cells/getrow/)(int) | (**Obsolete.**) Obtient l'élément [`Row`](../row/) à l'index de ligne de cellule spécifié. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator/)() | (**Obsolete.**) Obtient l'énumérateur des lignes. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight)(int) | Obtient la hauteur d'une ligne spécifiée, en points. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight_1)(int, bool, CellsUnitType) | Obtient la hauteur de la ligne. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch/)(int) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel/)(int) | Obtient la hauteur d'une ligne spécifiée en unité de pixel. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint/)(int) | (**Obsolete.**) Obtient la hauteur d'origine de la ligne en unité de point si la ligne est masquée |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel/)(int) | Obtenez la largeur dans différents types de vue. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight/)(int) | Obtient la hauteur d'une ligne spécifiée. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch/)(int) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns)(int, int) | Regroupe les colonnes. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns_1)(int, int, bool) | Regroupe les colonnes. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows)(int, int) | Regroupe les lignes. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows_1)(int, int, bool) | Regroupe les lignes. |
| [HideColumn](../../aspose.cells/cells/hidecolumn/)(int) | Masque une colonne. |
| [HideColumns](../../aspose.cells/cells/hidecolumns/)(int, int) | Masque plusieurs colonnes. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail/)(bool, int) | Réduit les lignes/colonnes groupées. |
| [HideRow](../../aspose.cells/cells/hiderow/)(int) | Masque une ligne. |
| [HideRows](../../aspose.cells/cells/hiderows/)(int, int) | Masque plusieurs lignes. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_1)(double[], int, int, bool) | Importe un tableau de doubles dans une feuille de calcul. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_3)(int[], int, int, bool) | Importe un tableau d'entiers dans une feuille de calcul. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_5)(string[], int, int, bool) | Importe un tableau de chaînes dans une feuille de calcul. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist/)(ArrayList, int, int, bool) | Importe une ArrayList de données dans une feuille de calcul. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv)(Stream, TxtLoadOptions, int, int) | Importe un fichier CSV dans les cellules. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_2)(string, TxtLoadOptions, int, int) | Importe un fichier CSV dans les cellules. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_1)(Stream, string, bool, int, int) | Importe un fichier CSV dans les cellules. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_3)(string, string, bool, int, int) | Importe un fichier CSV dans les cellules. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Importe des objets personnalisés. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Importe des objets personnalisés. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_3)(IDataReader, int, int) | Importe des données d'un objet IDataReader. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_1)(DataTable, int, int, ImportTableOptions) | Importe des données d'une table de données personnalisée. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_2)(DataView, int, int, ImportTableOptions) | Importe des données d'une vue de données. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Importe des données d'une table de données personnalisée. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_4)(IDataReader, int, int, ImportTableOptions) | Importe des données d'un objet IDataReader. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid)(DataGrid, int, int, bool) | Importe un DataGrid dans une feuille de calcul. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Importe un DataGrid dans une feuille de calcul. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Importe un DataGrid dans une feuille de calcul. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring/)(DataGrid, int, int, bool) | Importe un DataGrid dans une feuille de calcul. Cette méthode ne tente pas de convertir le texte en valeurs numériques. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow/)(DataRow, int, int) | Importe une DataRow dans le fichier Excel. |
| [ImportDataView](../../aspose.cells/cells/importdataview/)(DataView, int, int) | Importe une DataView dans une feuille de calcul. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray/)(string[], int, int, bool) | Importe un tableau de formules dans une feuille de calcul. |
| [ImportGridView](../../aspose.cells/cells/importgridview/)(GridView, int, int, ImportTableOptions) | Importe une vue de grille dans ces cellules. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray)(object[], int, int, bool) | Importe un tableau de données dans une feuille de calcul. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray_1)(object[], int, int, bool, int) | Importe un tableau de données dans une feuille de calcul. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn)(int) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn_1)(int, bool) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns)(int, int) | Insère plusieurs colonnes dans la feuille de calcul. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_2)(int, int, bool) | Insère plusieurs colonnes dans la feuille de calcul. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_1)(int, int, InsertOptions) | Insère plusieurs colonnes dans la feuille de calcul. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells/)(Range, int, int, ShiftType) | Insérer la plage découpée. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange)(CellArea, ShiftType) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_1)(CellArea, int, ShiftType) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_2)(CellArea, int, ShiftType, bool) | Insère une plage de cellules et décale les cellules selon l'option de décalage. |
| [InsertRow](../../aspose.cells/cells/insertrow/)(int) | Insère une nouvelle ligne dans la feuille de calcul. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows)(int, int) | Insère plusieurs lignes dans la feuille de calcul. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_2)(int, int, bool) | Insère plusieurs lignes dans la feuille de calcul. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_1)(int, int, InsertOptions) | Insère plusieurs lignes dans la feuille de calcul. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn/)(int) | Vérifie si la colonne donnée est vide (ne contient aucune donnée). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden/)(int) | Vérifie si une colonne à l'index donné est masquée. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled/)(int, int, int, int) | Vérifie si la plage peut être supprimée. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden/)(int) | Vérifie si une ligne à l'index donné est masquée. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap/)(string, int, int, string) | Lien vers une carte XML. |
| [Merge](../../aspose.cells/cells/merge/#merge)(int, int, int, int) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [Merge](../../aspose.cells/cells/merge/#merge_1)(int, int, int, int, bool) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [Merge](../../aspose.cells/cells/merge/#merge_2)(int, int, int, int, bool, bool) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [MoveRange](../../aspose.cells/cells/moverange/)(CellArea, int, int) | Déplace la plage. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates)() | Supprime les lignes en double dans la feuille. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_1)(int, int, int, int) | Supprime les valeurs en double dans la plage. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_2)(int, int, int, int, bool, int[]) | Supprime les données en double de la plage. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas/)() | Supprime toutes les formules et les remplace par la valeur de la formule. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting/)(CellArea) | Récupère les paramètres de sous-totaux de la plage. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth/)(int, double) | Définit la largeur de la colonne spécifiée en mode normal. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch/)(int, double) | Définit la largeur de la colonne en pouces en mode normal. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel/)(int, int) | Définit la largeur de la colonne en pixels en mode normal. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight/)(int, double) | Définit la hauteur de la ligne spécifiée. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch/)(int, double) | Définit la hauteur de la ligne en pouces. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel/)(int, int) | Définit la hauteur de la ligne en unités de pixels. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel/)(int, int) | Définit la largeur de la colonne dans différentes vues. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail/)(bool, int) | Développe les lignes/colonnes groupées. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Crée des sous‑totaux pour la plage. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Crée des sous‑totaux pour la plage. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns/)(int, int, int, TxtLoadOptions) | Divise le contenu de la colonne spécifiée en plusieurs colonnes.. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns/)(int, int) | Dégroupe les colonnes. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows)(int, int) | Dégroupe les lignes. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows_1)(int, int, bool) | Dégroupe les lignes. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn/)(int, double) | Dévoile une colonne |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns/)(int, int, double) | Dévoile plusieurs colonnes. |
| [UnhideRow](../../aspose.cells/cells/unhiderow/)(int, double) | Dévoile une ligne. |
| [UnhideRows](../../aspose.cells/cells/unhiderows/)(int, int, double) | Dévoile les lignes cachées. |
| [UnMerge](../../aspose.cells/cells/unmerge/)(int, int, int, int) | Démarque une plage spécifiée de cellules fusionnées. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDemo
    {
        public static void CellsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la hauteur de ligne par défaut
            cells.StandardHeight = 20;
            // Définir la hauteur de ligne
            cells.SetRowHeight(2, 20.5);

            // Définir la largeur de colonne par défaut
            cells.StandardWidth = 15;
            // Définir la largeur de colonne
            cells.SetColumnWidth(3, 12.57);

            // Fusionner des cellules
            cells.Merge(5, 4, 2, 2);

            // Attribuer des valeurs aux cellules
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(1);
            cells[0, 2].PutValue("abc");

            // Exporter des données
            object[,] arr = cells.ExportArray(0, 0, 10, 10);

            // Démontrer certaines propriétés
            Console.WriteLine("Total Cells Count: " + cells.Count);
            Console.WriteLine("Total Cells Count (Large): " + cells.CountLarge);
            Console.WriteLine("Min Row with Data: " + cells.MinDataRow);
            Console.WriteLine("Max Row with Data: " + cells.MaxDataRow);
            Console.WriteLine("Min Column with Data: " + cells.MinDataColumn);
            Console.WriteLine("Max Column with Data: " + cells.MaxDataColumn);

            // Parcourir les cellules
            IEnumerator enumerator = cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Enregistrez le classeur
            workbook.Save("CellsExample.xlsx");
            workbook.Save("CellsExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


