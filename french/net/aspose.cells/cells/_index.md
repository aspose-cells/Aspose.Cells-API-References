---
title: Cells
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule une collection dobjets pertinents pour les cellules tels queCell./cell Row./row ...etc.
type: docs
weight: 300
url: /fr/net/aspose.cells/cells/
---
## Cells class

Encapsule une collection d'objets pertinents pour les cellules, tels que[`Cell`](../cell) ,[`Row`](../row) ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns) { get; } | Obtient la collection de[`Column`](../column) objets qui représentent les colonnes individuelles dans cette feuille de calcul. |
| [Count](../../aspose.cells/cells/count) { get; } | Obtient le nombre total d'objets Cell instanciés. |
| [CountLarge](../../aspose.cells/cells/countlarge) { get; } | Obtient le nombre total d'objets Cell instanciés. |
| [FirstCell](../../aspose.cells/cells/firstcell) { get; } | Obtient la première cellule de cette feuille de calcul. |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched) { get; set; } | Indique que la hauteur de ligne et la hauteur de police par défaut correspondent à |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden) { get; set; } | Indique si la ligne est masquée par défaut. |
| [Item](../../aspose.cells/cells/item) { get; } | Obtient le[`Cell`](../cell) élément à l'index de ligne de cellule et à l'index de colonne spécifiés. (2 indexers) |
| [LastCell](../../aspose.cells/cells/lastcell) { get; } | Obtient la dernière cellule de cette feuille de calcul. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn) { get; } | Index de colonne minimum des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'y a été instanciée). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn) { get; } | Index de colonne maximal de la cellule contenant des données. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow) { get; } | Index de ligne maximal de la cellule contenant des données. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange) { get; } | Obtient la plage maximale qui inclut les données, les cellules fusionnées et les formes. |
| [MaxRow](../../aspose.cells/cells/maxrow) { get; } | Index de ligne maximal de la cellule contenant des données ou un style. |
| [MemorySetting](../../aspose.cells/cells/memorysetting) { get; set; } | Obtient ou définit l'option d'utilisation de la mémoire pour ces cellules. |
| [MergedCells](../../aspose.cells/cells/mergedcells) { get; } | Obtient la collection de cellules fusionnées. |
| [MinColumn](../../aspose.cells/cells/mincolumn) { get; } | Index de colonne minimum des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'y a été instanciée). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn) { get; } | Index de colonne minimum de la cellule contenant des données. |
| [MinDataRow](../../aspose.cells/cells/mindatarow) { get; } | Index de ligne minimum de la cellule contenant des données. |
| [MinRow](../../aspose.cells/cells/minrow) { get; } | Index de ligne minimum de la cellule contenant des données ou un style. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading) { get; set; } | Obtient ou définit si le modèle de données des cellules doit prendre en charge la lecture multi-thread. La valeur par défaut de cette propriété est false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields) { get; } | Obtient la liste des champs de ods. |
| [PreserveString](../../aspose.cells/cells/preservestring) { get; set; } | Obtient ou définit une valeur indiquant si toutes les valeurs de la feuille de calcul sont conservées sous forme de chaînes. La valeur par défaut est false. |
| [Ranges](../../aspose.cells/cells/ranges) { get; } | Obtient la collection de[`Range`](../range)objets créés au moment de l'exécution. |
| [Rows](../../aspose.cells/cells/rows) { get; } | Obtient la collection de[`Row`](../row) objets qui représentent les lignes individuelles de cette feuille de calcul. |
| [StandardHeight](../../aspose.cells/cells/standardheight) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en unités de points. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pouces. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels) { get; set; } | Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en pixels. |
| [StandardWidth](../../aspose.cells/cells/standardwidth) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en unités de caractères. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en pouces. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels) { get; set; } | Obtient ou définit la largeur de colonne par défaut dans la feuille de calcul, en unités de pixels. |
| [Style](../../aspose.cells/cells/style) { get; set; } | Obtient et définit le style par défaut. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange)(Range) | Ajoute une référence d'objet de plage aux cellules |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle)(int, Style, StyleFlag) | Applique les formats pour une colonne entière. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle)(int, Style, StyleFlag) | Applique les formats pour une ligne entière. |
| [ApplyStyle](../../aspose.cells/cells/applystyle)(Style, StyleFlag) | Applique les formats pour une feuille de calcul entière. |
| [CheckCell](../../aspose.cells/cells/checkcell)(int, int) | Obtient le[`Cell`](../cell) élément ou null à l'index de ligne de cellule et à l'index de colonne spécifiés. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn)(int) | Obtient le[`Column`](../column) élément ou null à l'index de colonne spécifié. |
| [CheckRow](../../aspose.cells/cells/checkrow)(int) | Obtient le[`Row`](../row) élément ou à l'index de ligne de cellule spécifié. |
| [Clear](../../aspose.cells/cells/clear)() | Efface tous les objets de cellule et de ligne. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents)(CellArea) | Efface le contenu d'une plage. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents_1)(int, int, int, int) | Efface le contenu d'une plage. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats)(CellArea) | Efface le formatage d'une plage. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats_1)(int, int, int, int) | Efface le formatage d'une plage. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells)() | Efface toutes les plages fusionnées. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange)(CellArea) | Efface le contenu et la mise en forme d'une plage. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange_1)(int, int, int, int) | Efface le contenu et la mise en forme d'une plage. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue)() | Convertit les données de chaîne dans les cellules en valeur numérique si possible. |
| [CopyColumn](../../aspose.cells/cells/copycolumn)(Cells, int, int) | Copie les données et les formats d'une colonne entière. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns)(Cells, int, int, int) | Copie les données et les formats d'une colonne entière. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_2)(Cells, int, int, int, int) | Copie les données et les formats de toutes les colonnes. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_1)(Cells, int, int, int, PasteOptions) | Copie les données et les formats d'une colonne entière. |
| [CopyRow](../../aspose.cells/cells/copyrow)(Cells, int, int) | Copie les données et les formats d'une ligne entière. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows)(Cells, int, int, int) | Copie les données et les formats de certaines lignes entières. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_1)(Cells, int, int, int, CopyOptions) | Copie les données et les formats de certaines lignes entières. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Copie les données et les formats de certaines lignes entières. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_2)(string) | Crée un[`Range`](../range) objet à partir d'une adresse de la plage. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_3)(string, string) | Crée un[`Range`](../range) objet d'une plage de cellules. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange)(int, int, bool) | Crée un[`Range`](../range) objet à partir de lignes de cellules ou de colonnes de cellules. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_1)(int, int, int, int) | Crée un[`Range`](../range) objet d'une plage de cellules. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns)() | Supprimer toutes les colonnes vides qui ne contiennent aucune donnée. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns_1)(DeleteOptions) | Supprimer toutes les colonnes vides qui ne contiennent aucune donnée. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows)() | Supprimer toutes les lignes vides qui ne contiennent aucune donnée. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows_1)(DeleteOptions) | Supprimer toutes les lignes vides qui ne contiennent aucune donnée. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn)(int) | Supprime une colonne. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn_1)(int, bool) | Supprime une colonne. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns)(int, int, bool) | Supprime plusieurs colonnes. |
| [DeleteRange](../../aspose.cells/cells/deleterange)(int, int, int, int, ShiftType) | Supprime une plage de cellules et décale les cellules en fonction de l'option de décalage. |
| [DeleteRow](../../aspose.cells/cells/deleterow)(int) | Supprime une ligne. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows)(int, int) | Supprime plusieurs lignes. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows_1)(int, int, bool) | Supprime plusieurs lignes dans la feuille de calcul. |
| [Dispose](../../aspose.cells/cells/dispose)() | Effectue des tâches définies par l'application associées à la libération, à la libération ou à la réinitialisation des ressources non gérées. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn)(short) | Récupère la dernière cellule de cette colonne. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn_1)(int, int, short, short) | Obtient la dernière cellule avec l'index de colonne maximal dans cette plage. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow)(int) | Obtient la dernière cellule de cette ligne. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow_1)(int, int, int, int) | Obtient la dernière cellule avec l'index de ligne maximal dans cette plage. |
| [ExportArray](../../aspose.cells/cells/exportarray)(int, int, int, int) | Exporte les données dans le[`Cells`](../cells) collection à un objet tableau à deux dimensions. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable)(int, int, int, int) | Exporte les données dans le[`Cells`](../cells) collecte à unDataTable objet. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_2)(int, int, int, int, bool) | Exporte les données dans le[`Cells`](../cells) collecte à unDataTable objet. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Exporte les données dans le[`Cells`](../cells) collecte à unDataTable objet. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring)(int, int, int, int) | Exporte les données dans le[`Cells`](../cells) collecte à unDataTable objet. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring_1)(int, int, int, int, bool) | Exporte les données dans le[`Cells`](../cells) collecte à unDataTable objet. |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray)(int, int, int, int) | Exporte le type de valeur de cellule dans le[`Cells`](../cells) collection à un objet tableau à deux dimensions. |
| [Find](../../aspose.cells/cells/find#find)(object, Cell) | Trouve la cellule contenant l'objet d'entrée. |
| [Find](../../aspose.cells/cells/find#find_1)(object, Cell, FindOptions) | Trouve la cellule contenant l'objet d'entrée. |
| [GetCell](../../aspose.cells/cells/getcell)(int, int) | Obtient le[`Cell`](../cell) élément ou null à l'index de ligne de cellule et à l'index de colonne spécifiés. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle)(int, int) | Obtenir le style de la cellule donnée. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth)(int) | Obtient la largeur de la colonne spécifiée en vue normale |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch)(int) | Obtient la largeur de la colonne spécifiée en vue normale, en unités de pouces. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel)(int) | Obtient la largeur de la colonne spécifiée en vue normale, en unités de pixel. |
| [GetDependents](../../aspose.cells/cells/getdependents)(bool, int, int) | Obtenir toutes les cellules qui font référence à la cellule spécifique. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation)(int, int, bool) | Obtient toutes les cellules dont le résultat calculé dépend d'une cellule spécifique. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator)() | Obtient l'énumérateur de cellules. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel)(int) | Obtient le niveau hiérarchique (basé sur zéro) de la colonne. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel)(int) | Obtient le niveau hiérarchique (basé sur zéro) de la ligne. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow)(int) | Obtient le dernier index de ligne de la cellule qui contient des données dans la colonne spécifiée. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel)() | Obtient le niveau hiérarchique maximal des colonnes groupées (base zéro). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel)() | Obtient le niveau maximal de plan de lignes groupées (basé sur zéro). |
| [GetRow](../../aspose.cells/cells/getrow)(int) | Obtient le[`Row`](../row) élément à l'index de ligne de cellule spécifié. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator)() | Obtient l'énumérateur de lignes. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight)(int) | Obtient la hauteur d'une ligne spécifiée. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch)(int) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel)(int) | Obtient la hauteur d'une ligne spécifiée en unité de pixel. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint)(int) | Obtient la hauteur de la ligne d'origine en unité de point si la ligne est masquée |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel)(int) | Obtenez la largeur dans différents types de vue. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight)(int) | Obtient la hauteur d'une ligne spécifiée. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch)(int) | Obtient la hauteur d'une ligne spécifiée en pouces. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns)(int, int) | Regroupe les colonnes. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns_1)(int, int, bool) | Regroupe les colonnes. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows)(int, int) | Regroupe les lignes. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows_1)(int, int, bool) | Regroupe les lignes. |
| [HideColumn](../../aspose.cells/cells/hidecolumn)(int) | Masque une colonne. |
| [HideColumns](../../aspose.cells/cells/hidecolumns)(int, int) | Masquer plusieurs colonnes. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail)(bool, int) | Réduit les lignes/colonnes groupées. |
| [HideRow](../../aspose.cells/cells/hiderow)(int) | Masque une ligne. |
| [HideRows](../../aspose.cells/cells/hiderows)(int, int) | Masque plusieurs lignes. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_1)(double[], int, int, bool) | Importe un tableau de doubles dans une feuille de calcul. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_3)(int[], int, int, bool) | Importe un tableau d'entiers dans une feuille de calcul. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_5)(string[], int, int, bool) | Importe un tableau de chaînes dans une feuille de calcul. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist)(ArrayList, int, int, bool) | Importe un tableau de données dans une feuille de calcul. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv)(Stream, TxtLoadOptions, int, int) | Importer un fichier CSV dans les cellules. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_2)(string, TxtLoadOptions, int, int) | Importer un fichier CSV dans les cellules. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_1)(Stream, string, bool, int, int) | Importer un fichier CSV dans les cellules. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_3)(string, string, bool, int, int) | Importer un fichier CSV dans les cellules. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Importe des objets personnalisés. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Importe des objets personnalisés. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_3)(IDataReader, int, int) | Importe des données à partir d'unIDataReader objet. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_1)(DataTable, int, int, ImportTableOptions) | Importer des données à partir d'un tableau de données personnalisé. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_2)(DataView, int, int, ImportTableOptions) | Importer des données à partir de la vue des données. |
| [ImportData](../../aspose.cells/cells/importdata#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Importer des données à partir d'un tableau de données personnalisé. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_4)(IDataReader, int, int, ImportTableOptions) | Importe des données à partir d'unIDataReader objet. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid)(DataGrid, int, int, bool) | Importe unDataGrid dans une feuille de calcul. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Importe unDataGrid dans une feuille de calcul. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Importe unDataGrid dans une feuille de calcul. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring)(DataGrid, int, int, bool) | Importe unDataGrid dans une feuille de travail. Cette méthode n'essaie pas de convertir le texte en valeurs numériques. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow)(DataRow, int, int) | Importe un DataRow dans le fichier Excel. |
| [ImportDataView](../../aspose.cells/cells/importdataview#importdataview_3)(DataView, int, int) | Importe unDataView dans une feuille de calcul. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray)(string[], int, int, bool) | Importe un tableau de formules dans une feuille de calcul. |
| [ImportGridView](../../aspose.cells/cells/importgridview)(GridView, int, int, ImportTableOptions) | Importe une vue de grille dans ces cellules. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray)(object[], int, int, bool) | Importe un tableau de données dans une feuille de calcul. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray_1)(object[], int, int, bool, int) | Importe un tableau de données dans une feuille de calcul. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn)(int) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn_1)(int, bool) | Insère une nouvelle colonne dans la feuille de calcul. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns)(int, int) | Insère des colonnes dans la feuille de calcul. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns_1)(int, int, bool) | Insère des colonnes dans la feuille de calcul. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells)(Range, int, int, ShiftType) | Insérer la plage de coupe. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange)(CellArea, ShiftType) | Insère une plage de cellules et décale les cellules en fonction de l'option de décalage. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_1)(CellArea, int, ShiftType) | Insère une plage de cellules et décale les cellules en fonction de l'option de décalage. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_2)(CellArea, int, ShiftType, bool) | Insère une plage de cellules et décale les cellules en fonction de l'option de décalage. |
| [InsertRow](../../aspose.cells/cells/insertrow)(int) | Insère une nouvelle ligne dans la feuille de calcul. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows)(int, int) | Insère plusieurs lignes dans la feuille de calcul. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_2)(int, int, bool) | Insère plusieurs lignes dans la feuille de calcul. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_1)(int, int, InsertOptions) | Insère plusieurs lignes dans la feuille de calcul. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn)(int) | Vérifie si la colonne donnée est vide (ne contient aucune donnée). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden)(int) | Vérifie si une colonne à un index donné est masquée. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled)(int, int, int, int) | Vérifiez si la plage peut être supprimée. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden)(int) | Vérifie si une ligne à un index donné est masquée. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap)(string, int, int, string) | Lien vers une carte xml. |
| [Merge](../../aspose.cells/cells/merge#merge)(int, int, int, int) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [Merge](../../aspose.cells/cells/merge#merge_1)(int, int, int, int, bool) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [Merge](../../aspose.cells/cells/merge#merge_2)(int, int, int, int, bool, bool) | Fusionne une plage de cellules spécifiée en une seule cellule. |
| [MoveRange](../../aspose.cells/cells/moverange)(CellArea, int, int) | Déplace la plage. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates)() | Supprime les lignes en double dans la feuille. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_1)(int, int, int, int) | Supprime les valeurs en double dans la plage. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_2)(int, int, int, int, bool, int[]) | Supprime les données en double de la plage. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas)() | Supprime toutes les formules et les remplace par la valeur de la formule. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting)(CellArea) | Récupère le réglage des sous-totaux de la plage. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth)(int, double) | Définit la largeur de la colonne spécifiée en vue normale. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch)(int, double) | Définit la largeur de la colonne en pouces en vue normale. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel)(int, int) | Définit la largeur de la colonne en pixels en vue normale. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight)(int, double) | Définit la hauteur de la ligne spécifiée. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch)(int, double) | Définit la hauteur de ligne en pouces. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel)(int, int) | Définit la hauteur de ligne en pixels. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel)(int, int) | Définit la largeur de la colonne dans différentes vues. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail)(bool, int) | Développe les lignes/colonnes groupées. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Crée des sous-totaux pour la plage. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Crée des sous-totaux pour la plage. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns)(int, int, int, TxtLoadOptions) | Divise le texte de la colonne en colonnes. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns)(int, int) | Dissocie les colonnes. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows)(int, int) | Dissocie les lignes. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows_1)(int, int, bool) | Dissocie les lignes. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn)(int, double) | Affiche une colonne |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns)(int, int, double) | Afficher plusieurs colonnes. |
| [UnhideRow](../../aspose.cells/cells/unhiderow)(int, double) | Affiche une ligne. |
| [UnhideRows](../../aspose.cells/cells/unhiderows)(int, int, double) | Affiche les lignes masquées. |
| [UnMerge](../../aspose.cells/cells/unmerge)(int, int, int, int) | Annule la fusion d'une plage spécifiée de cellules fusionnées. |

### Exemples

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Définir la hauteur de ligne par défaut
cells.StandardHeight = 20;
//Définir la hauteur de la ligne
cells.SetRowHeight(2, 20.5);

//Définir la largeur de colonne par défaut
cells.StandardWidth = 15;
//Définir la largeur de la colonne
cells.SetColumnWidth(3, 12.57);

//Fusionner des cellules
cells.Merge(5, 4, 2, 2);

//Mettez des valeurs dans les cellules
cells[0, 0].PutValue(true);
cells[0, 1].PutValue(1);
cells[0, 2].PutValue("abc");

//Exporter des données
object[,] arr = cells.ExportArray(0, 0, 10, 10);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Définir la hauteur de ligne par défaut
cells.StandardHeight = 20
'Définir la hauteur de ligne
cells.SetRowHeight(2, 20.5)

'Définir la largeur de colonne par défaut
cells.StandardWidth = 15
'Définir la largeur de la colonne
cells.SetColumnWidth(3, 12.57)

'Fusionner des cellules
cells.Merge(5, 4, 2, 2)

'Exporter des données
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
