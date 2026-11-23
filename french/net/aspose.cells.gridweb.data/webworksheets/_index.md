---
title: "Classe WebWorksheets"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.WebWorksheets."
type: docs
url: /fr/net/aspose.cells.gridweb.data/webworksheets/
---
## WebWorksheets class

```csharp
[Obsolete("This class is obsolete; use  GridWorksheetCollection instead")]
public class WebWorksheets : ICollection, ISerializable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WebWorksheets](webworksheets/)(MainWeb, GridWorksheetCollection) |  |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActiveSheet](../../aspose.cells.gridweb.data/webworksheets/activesheet/) { get; } |  |
| [ActiveSheetIndex](../../aspose.cells.gridweb.data/webworksheets/activesheetindex/) { get; set; } |  |
| [Count](../../aspose.cells.gridweb.data/webworksheets/count/) { get; } |  |
| [DefaultFontName](../../aspose.cells.gridweb.data/webworksheets/defaultfontname/) { get; set; } |  |
| [DefaultFontSize](../../aspose.cells.gridweb.data/webworksheets/defaultfontsize/) { get; set; } |  |
| [IsFixedSize](../../aspose.cells.gridweb.data/webworksheets/isfixedsize/) { get; } | Obtient une valeur indiquant si la collection a une taille fixe. |
| [IsReadOnly](../../aspose.cells.gridweb.data/webworksheets/isreadonly/) { get; } | Obtient une valeur indiquant si l'IList est en lecture seule. |
| [IsSynchronized](../../aspose.cells.gridweb.data/webworksheets/issynchronized/) { get; } | Obtient une valeur indiquant si l'accès à l'ICollection est synchronisé (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/webworksheets/item/) { get; } | Obtient l'élément Worksheet à l'index spécifié. (2 indexeurs) |
| [PivotCaches](../../aspose.cells.gridweb.data/webworksheets/pivotcaches/) { get; } | Obtient l'objet de collection PivotCache |
| [PivotTables](../../aspose.cells.gridweb.data/webworksheets/pivottables/) { get; } | Obtient l'objet de collection pivotTable. |
| [SyncRoot](../../aspose.cells.gridweb.data/webworksheets/syncroot/) { get; } | Obtient un objet pouvant être utilisé pour synchroniser l'accès à l'ICollection. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add)() | Ajoute une feuille de calcul à la collection. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_1)(object) | Ajoute un objet feuille. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_2)(string) | Ajoute une feuille de calcul à la collection. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_1)(int) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_2)(string) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy)(WebWorksheet) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [Clear](../../aspose.cells.gridweb.data/webworksheets/clear/)() | Efface toutes les feuilles de calcul. |
| [Contains](../../aspose.cells.gridweb.data/webworksheets/contains/)(object) | Indique si la collection contient la feuille. |
| [CopyTo](../../aspose.cells.gridweb.data/webworksheets/copyto/)(Array, int) | Copie le contenu dans un tableau. |
| [GetEnumerator](../../aspose.cells.gridweb.data/webworksheets/getenumerator/)() |  |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview)(DataView, TableItemStyle, TableItemStyle) | Importe depuis un DataView. Crée automatiquement une feuille avec le nom de table du DataView. |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview_1)(DataView, TableItemStyle, TableItemStyle, string, int, int) | Importe depuis un DataView vers la feuille et la position spécifiées. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile)(Stream) | Importe depuis un flux de fichier Excel, y compris un flux de fichier disque ou un flux mémoire. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile_1)(string) | Importe depuis un fichier Excel. |
| [IndexOf](../../aspose.cells.gridweb.data/webworksheets/indexof/)(object) | Obtient l'index de la feuille. |
| [Insert](../../aspose.cells.gridweb.data/webworksheets/insert/)(int, string) | Insère une feuille à l'index. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile)(Stream) | Charge les données depuis un flux de fichier CSV. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile_1)(string) | Charge les données depuis un fichier CSV. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile)(Stream) | Charge les données depuis un flux de fichier HTML. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile_1)(string) | Charge les données depuis un fichier HTML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Charge les données depuis un flux de fichier SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Charge les données depuis un fichier SpreadSheetML. |
| [Remove](../../aspose.cells.gridweb.data/webworksheets/remove/)(object) | Supprime une feuille. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat)(int) | Supprime une feuille à l'index. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat_1)(string) | Supprime l'élément à un nom spécifié. |
| [RunAllFormulas](../../aspose.cells.gridweb.data/webworksheets/runallformulas/)() | Exécute les formules de toutes les cellules. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile)(Stream) | Enregistre les données dans un flux de fichier CSV. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile_1)(string) | Enregistre les données dans un fichier CSV. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile)(Stream) | Enregistre les données dans un flux de fichier HTML. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile_1)(string) | Enregistre les données dans un fichier HTML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Enregistre les données dans un flux de fichier SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Enregistre les données dans un fichier SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile)(Stream) | Enregistre les feuilles de calcul dans un flux de fichier Excel, y compris le flux d'E/S disque ou le flux mémoire. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_2)(string) | Enregistre les feuilles de calcul dans un fichier Excel au format Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Enregistre les feuilles de calcul dans un fichier Excel. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_3)(string, GridSaveFormat) | Enregistre les feuilles de calcul dans un fichier Excel. |

### Remarques

NOTE: Cette classe est maintenant obsolète. Veuillez utiliser GridWorksheetCollection à la place. Cette classe sera supprimée après 6 mois à compter d'août 2014. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


