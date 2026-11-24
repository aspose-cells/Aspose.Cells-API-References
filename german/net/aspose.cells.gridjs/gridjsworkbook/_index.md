---
title: "Klasse GridJsWorkbook"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridJs.GridJsWorkbook Klasse. Stellt die Haupteinstiegsklasse für GridJs dar"
type: docs
url: /de/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Stellt die Haupt‑Einstiegsklasse für GridJs dar.

```csharp
public class GridJsWorkbook
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook/)() | Erstellt eine neue Instanz von GridJsWorkbook. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CacheDirectory](../../aspose.cells.gridjs/gridjsworkbook/cachedirectory/) { get; set; } | Liest/Setzt das Cache-Verzeichnis zum Speichern von Tabellenkalkulationsdateien. Wenn dies nicht gesetzt ist, verwenden wir die statische Eigenschaft von [`FileCacheDirectory`](../config/filecachedirectory/) oder [`CacheImp`](./cacheimp/). |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings/) { get; set; } | Stellt die Einstellungen der Arbeitsmappe dar. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback/) { get; set; } | Liest oder setzt den Warn-Callback für den Import von Dateien. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [BurnRedactionFile](../../aspose.cells.gridjs/gridjsworkbook/burnredactionfile/)(string, string) | Führt (wendet) alle Redaktionsoperationen im Arbeitsbuch aus, indem Redaktionsformen und deren Zielformen entfernt oder der Inhalt des Zielzellenbereichs gelöscht wird. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsworkbook/checkincacheforcollaborative/)(string) | Prüft, ob die Arbeitsmappeninstanz im Speicher-Cache ist. Diese Methode wird nur im kollaborativen Modus angewendet. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsworkbook/clearalljsoncache/)() | Alle JSON-Cache löschen |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsworkbook/clearjsoncacheforuid/)(string) | JSON-Cache basierend auf UID löschen (für Szenarien wie UpdateCell, bei denen nur die UID vorhanden ist) |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape/)(string, string) | Kopiert Bild oder Form. |
| [Dispose](../../aspose.cells.gridjs/gridjsworkbook/dispose/)() | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson/)(string) | Liest die Fehlermeldungszeichenkette im JSON-Format. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson)() | Liest JSON-Zeichenkette aus den Speicherdaten, der Standarddateiname im JSON ist: book1. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson_1)(string) | Liest JSON-Zeichenkette aus den Speicherdaten, legt den Ausgabedateinamen im JSON fest. |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder/)(string, string) | Liest JSON-Zeichenkette aus den Speicherdaten, legt den Ausgabedateinamen im JSON fest. |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid/)(string, string) | Liefert den JSON‑String der Datei aus dem Cache anhand der angegebenen eindeutigen ID, setzt den Ausgabedateinamen im JSON. |
| [GetOle](../../aspose.cells.gridjs/gridjsworkbook/getole/)(string, string, int, out string) | Liefert die Byte‑Array‑Daten des eingebetteten OLE‑Objekts. |
| [GetSheetJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getsheetjsonwithcache/)(string, string, string) | JSON des angegebenen Blatts abrufen (mit Cache) |
| [GetWorkbookJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getworkbookjsonwithcache/)(string, string) | JSON der gesamten Arbeitsmappe abrufen (mit Cache) |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_3)(string) | Importiert die Excel-Datei vom Dateipfad. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile)(Workbook) | Importiert die Excel-Datei aus dem Arbeitsmappenobjekt. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_1)(Stream, GridLoadFormat) | Importiert die Excel-Datei aus einem Dateistream mit Ladeformat. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_7)(string, string) | Importiert die Excel-Datei vom Dateipfad. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_4)(string, Workbook) | Importiert die Excel-Datei aus dem Arbeitsmappenobjekt. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_2)(Stream, GridLoadFormat, string) | Importiert die Excel-Datei aus einem Dateistream mit Ladeformat und Öffnungspasswort. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_5)(string, Stream, GridLoadFormat) | Importiert die Excel-Datei aus einem Dateistream. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_8)(string, string, string) | Importiert die Excel-Datei vom Dateipfad und Öffnungspasswort. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Importiert die Excel-Datei aus einem Dateistream mit Ladeformat und Öffnungspasswort. |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson/)(string) | Importiert die Excel-Datei aus einer JSON-Formatzeichenkette. |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage/)(string, string, Stream, string) | Fügt ein Bild im Arbeitsblatt aus einem Dateistream oder einer URL ein (entweder der Dateistream oder die URL muss bereitgestellt werden) oder fügt eine Form ein, wenn p.type einer der AutoShapeType ist. |
| [JsonToStream](../../aspose.cells.gridjs/gridjsworkbook/jsontostream/)(Stream, string, string) | Erstellt JSON aus der im Speicher befindlichen Arbeitsmappe und schreibt es in den angegebenen Stream. Optional wird das erzeugte JSON zwischengespeichert, um spätere Abrufe zu beschleunigen. Wesentliche Unterschiede zu JsonToStreamByUid: - Diese Methode verwendet den aktuellen im Speicher befindlichen Arbeitsmappenstatus (wb-Feld) - JsonToStreamByUid lädt die Arbeitsmappe aus .cells-Cache-Dateien auf der Festplatte neu - Verwenden Sie diese Methode, wenn Sie den aktuellen Arbeitsmappenstatus nach Änderungen exportieren möchten - Verwenden Sie JsonToStreamByUid, wenn Sie JSON aus einem zuvor zwischengespeicherten Dateistatus neu generieren müssen. Caching‑Verhalten (wenn uid angegeben ist): - Prüft den JSON-Cache vor der Erzeugung (L1 Speicher + L2 Festplatte) - Bei einem Cache‑Fehltreffer wird JSON aus der im Speicher befindlichen Arbeitsmappe erzeugt - Speichert das erzeugte JSON im Cache für zukünftige Anfragen. |
| [JsonToStreamByUid](../../aspose.cells.gridjs/gridjsworkbook/jsontostreambyuid/)(Stream, string, string) | Rufen Sie die JSON-Zeichenkette der Datei aus dem Cache mit der angegebenen eindeutigen ID ab, setzen Sie den Ausgabedateinamen in der JSON und schreiben Sie sie in den Stream. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingjson/)(string, string) | Liefert den JSON‑String des angegebenen Arbeitsblatts in der Datei aus dem Cache anhand der angegebenen eindeutigen ID. |
| [LazyLoadingStream](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingstream/)(Stream, string, string) | Rufen Sie die JSON-Zeichenkette des angegebenen Tabellenblatts in der Datei aus dem Cache mit der angegebenen eindeutigen ID ab und schreiben Sie sie in den Stream. |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson/)(string, string) | Wendet ein Batch-Update auf die Speicherdaten an. |
| [RedactFile](../../aspose.cells.gridjs/gridjsworkbook/redactfile/)(string, string, string[]) | Führt eine Redaktion einer Excel-Datei basierend auf einem Array von JSON-Operationen durch. |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename/)(string, string, string) | Speichert die Speicherdaten in die Cache-Datei mit dem angegebenen Dateinamen und setzt zudem das Öffnungspasswort, das Speicherformat basiert auf der Dateierweiterung des Dateinamens. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile)(Stream) | Speichert die Speicherdaten in den Stream, basierend auf dem Originaldateiformat. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile_1)(string) | Speichert die Speicherdaten im Dateipfad, falls die Datei eine Erweiterung hat, basiert das Speicherformat auf der Dateierweiterung. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml)(Stream) | Speichert die Speicherdaten in den Stream, das Speicherformat ist HTML. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml_1)(string) | Speichert die Speicherdaten im Dateipfad, das Speicherformat ist HTML. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf)(Stream) | Speichert die Speicherdaten in den Stream, das Speicherformat ist PDF. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf_1)(string) | Speichert die Speicherdaten im Dateipfad, das Speicherformat ist PDF. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx)(Stream) | Speichert die Speicherdaten in den Stream, das Speicherformat ist XLSX. |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx_1)(string) | Speichert die Speicherdaten im Dateipfad, das Speicherformat ist XLSX. |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload/)(GridInterruptMonitor, int) | Setzt InterruptMonitor für Ladevorgänge. |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave/)(GridInterruptMonitor) | Setzt InterruptMonitor für Speicheroperationen. |
| [SetTransParentView](../../aspose.cells.gridjs/gridjsworkbook/settransparentview/)(string, string, bool) | Setzt die Transparenz der Redaktionsformen im Arbeitsbuch. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsworkbook/translatesheetasync/)(string, string, ITextTranslator, string) | Übersetze alle Zeichenkettenwerte in die Zielsprache im Arbeitsblatt |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell/)(string, string) | Wendet die Aktualisierungsoperation an. |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat/)(string) | Ermittelt das Ladeformat anhand der Dateierweiterung. |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream/)(string, string, string) | Bild‑Stream abrufen. |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl/)(string, string, string) | Liefert die Bild‑URL. |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile/)(string) | Erzeugt eine neue eindeutige ID für den Dateicache anhand des angegebenen Dateinamens. |
| static [SetImageUrlBase](../../aspose.cells.gridjs/gridjsworkbook/setimageurlbase/)(string) | Setzt die Basis-Image‑Abruf‑URL vom Controller. |

## Felder

| Name | Beschreibung |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp/) | Benutzerdefinierte Implementierung für die Cache‑Speicherung. Wenn Sie den Cache im Stream‑Modus speichern möchten, müssen Sie ihn setzen und implementieren. |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine/) | Benutzerdefinierte Implementierung für die Berechnungs‑Engine. Wenn Sie benutzerdefinierte Berechnungen durchführen möchten, müssen Sie sie setzen und implementieren. |
| const [pictureType](../../aspose.cells.gridjs/gridjsworkbook/picturetype/) | Konstanter Wert für den Bildtyp. |
| static [UpdateMonitor](../../aspose.cells.gridjs/gridjsworkbook/updatemonitor/) | Liest/Setzt den Update‑Monitor, um Aktualisierungsvorgänge zu verfolgen. |

### Siehe auch

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


