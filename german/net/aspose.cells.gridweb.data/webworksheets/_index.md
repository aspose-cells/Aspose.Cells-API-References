---
title: "Klasse WebWorksheets"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.WebWorksheets-Klasse."
type: docs
url: /de/net/aspose.cells.gridweb.data/webworksheets/
---
## WebWorksheets class

```csharp
[Obsolete("This class is obsolete; use  GridWorksheetCollection instead")]
public class WebWorksheets : ICollection, ISerializable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [WebWorksheets](webworksheets/)(MainWeb, GridWorksheetCollection) |  |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActiveSheet](../../aspose.cells.gridweb.data/webworksheets/activesheet/) { get; } |  |
| [ActiveSheetIndex](../../aspose.cells.gridweb.data/webworksheets/activesheetindex/) { get; set; } |  |
| [Count](../../aspose.cells.gridweb.data/webworksheets/count/) { get; } |  |
| [DefaultFontName](../../aspose.cells.gridweb.data/webworksheets/defaultfontname/) { get; set; } |  |
| [DefaultFontSize](../../aspose.cells.gridweb.data/webworksheets/defaultfontsize/) { get; set; } |  |
| [IsFixedSize](../../aspose.cells.gridweb.data/webworksheets/isfixedsize/) { get; } | Liefert einen Wert, der angibt, ob die Sammlung eine feste Größe hat. |
| [IsReadOnly](../../aspose.cells.gridweb.data/webworksheets/isreadonly/) { get; } | Liefert einen Wert, der angibt, ob die IList schreibgeschützt ist. |
| [IsSynchronized](../../aspose.cells.gridweb.data/webworksheets/issynchronized/) { get; } | Liefert einen Wert, der angibt, ob der Zugriff auf die ICollection synchronisiert (thread-sicher) ist. |
| [Item](../../aspose.cells.gridweb.data/webworksheets/item/) { get; } | Liefert das Worksheet-Element am angegebenen Index. (2 Indexer) |
| [PivotCaches](../../aspose.cells.gridweb.data/webworksheets/pivotcaches/) { get; } | Liefert das PivotCache-Sammlungsobjekt |
| [PivotTables](../../aspose.cells.gridweb.data/webworksheets/pivottables/) { get; } | Liefert das pivotTable-Sammlungsobjekt. |
| [SyncRoot](../../aspose.cells.gridweb.data/webworksheets/syncroot/) { get; } | Liefert ein Objekt, das zum Synchronisieren des Zugriffs auf die ICollection verwendet werden kann. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add)() | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_1)(object) | Fügt ein Blatt-Objekt hinzu. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_2)(string) | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_1)(int) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_2)(string) | Fügt ein Arbeitsblatt zur Sammlung hinzu und kopiert Daten von einem bestehenden Arbeitsblatt. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy)(WebWorksheet) | Fügt ein Arbeitsblatt zur Sammlung hinzu und kopiert Daten von einem bestehenden Arbeitsblatt. |
| [Clear](../../aspose.cells.gridweb.data/webworksheets/clear/)() | Löscht alle Arbeitsblätter. |
| [Contains](../../aspose.cells.gridweb.data/webworksheets/contains/)(object) | Gibt an, ob die Sammlung das Blatt enthält. |
| [CopyTo](../../aspose.cells.gridweb.data/webworksheets/copyto/)(Array, int) | Kopiert Inhalte in ein Array. |
| [GetEnumerator](../../aspose.cells.gridweb.data/webworksheets/getenumerator/)() |  |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview)(DataView, TableItemStyle, TableItemStyle) | Importiert aus einem DataView. Erstellt automatisch ein Blatt mit dem Tabellennamen des DataView. |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview_1)(DataView, TableItemStyle, TableItemStyle, string, int, int) | Importiert aus einem DataView in das angegebene Blatt und die angegebene Position. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile)(Stream) | Importiert aus einem Excel-Dateistream, einschließlich Dateistream von Festplatte oder Speicherstream. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile_1)(string) | Importiert aus einer Excel-Datei. |
| [IndexOf](../../aspose.cells.gridweb.data/webworksheets/indexof/)(object) | Ermittelt den Index des Blatts. |
| [Insert](../../aspose.cells.gridweb.data/webworksheets/insert/)(int, string) | Fügt ein Blatt an dem Index ein. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile)(Stream) | Lädt Daten aus einem CSV-Datei-Stream. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile_1)(string) | Lädt Daten aus einer CSV-Datei. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile)(Stream) | Lädt Daten aus einem HTML-Datei-Stream. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile_1)(string) | Lädt Daten aus einer HTML-Datei. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Lädt Daten aus einem SpreadSheetML-Datei-Stream. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Lädt Daten aus einer SpreadSheetML-Datei. |
| [Remove](../../aspose.cells.gridweb.data/webworksheets/remove/)(object) | Entfernt ein Blatt. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat)(int) | Entfernt ein Blatt am Index. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat_1)(string) | Entfernt das Element mit einem angegebenen Namen. |
| [RunAllFormulas](../../aspose.cells.gridweb.data/webworksheets/runallformulas/)() | Führt die Formeln aller Zellen aus. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile)(Stream) | Speichert Daten in einen CSV-Datei-Stream. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile_1)(string) | Speichert Daten in einer CSV-Datei. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile)(Stream) | Speichert Daten in einen HTML-Datei-Stream. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile_1)(string) | Speichert Daten in einer HTML-Datei. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Speichert Daten in einen SpreadSheetML-Datei-Stream. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Speichert Daten in einer SpreadSheetML-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile)(Stream) | Speichert die Arbeitsblätter in einen Excel-Datei-Stream, einschließlich Festplatten‑IO‑Stream oder Speicher‑Stream. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_2)(string) | Speichert die Arbeitsblätter in einer Excel-Datei im Excel‑2003-Format. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_3)(string, GridSaveFormat) | Speichert die Arbeitsblätter in einer Excel-Datei. |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen GridWorksheetCollection. Diese Klasse wird nach 6 Monaten ab August 2014 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


