---
title: GridHtmlSaveOptions
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert die Optionen zum Speichern der HTML-Datei.
type: docs
weight: 250
url: /de/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Repräsentiert die Optionen zum Speichern der HTML-Datei.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor)() | Erstellt Optionen zum Speichern der HTML-Datei. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions#constructor_1)(GridSaveFormat) | Erstellt Optionen zum Speichern der HTML-Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory) { get; set; } | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur zum Speichern im HTML-Stream. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix) { get; set; } | Geben Sie das URL-Präfix von angehängten Dateien wie Bild in der HTML-Datei an. Nur zum Speichern im HTML-Stream. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder) { get; set; } | Der zwischengespeicherte Dateiordner wird verwendet, um einige große Daten zu speichern. |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata) { get; set; } | Machen Sie die Arbeitsmappe nach dem Speichern der Datei leer. |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory) { get; set; } | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis automatisch erstellt, bevor die Datei gespeichert wird. |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname) { get; set; } | Geben Sie den Namen der Standardschriftart zum Exportieren von HTML an, die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist, Wenn diese Eigenschaft null ist, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat, der Standardwert ist null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding) { get; set; } | Wenn nicht festgelegt, verwenden Sie Encoding.UTF8 als Standardcodierungstyp. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly) { get; set; } | Gibt an, ob die gesamte Arbeitsmappe in eine HTML-Datei exportiert wird. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea) { get; set; } | Ermittelt oder setzt den exportierenden CellArea des aktuell aktiven Arbeitsblatts. Wenn Sie dieses Attribut setzen, wird der Druckbereich des aktuell aktiven Arbeitsblatts ausgelassen. Nur der angegebene Bereich wird exportiert, wenn die Datei in HTML gespeichert wird. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines) { get; set; } | Gibt an, ob die Gitternetzlinien exportiert werden. Der Standardwert ist „false“. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings) { get; set; } | Gibt an, ob beim Speichern der Datei in HTML Überschriften exportiert werden. Der Standardwert ist „false“. Wenn Sie die HTML-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet) { get; set; } | Gibt an, ob der Inhalt des ausgeblendeten Arbeitsblatts exportiert wird. Der Standardwert ist wahr. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64) { get; set; } | Gibt an, ob Bilder im Base64-Format in HTML, MHTML oder EPUB gespeichert werden. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly) { get; set; } | Gibt an, ob nur der Druckbereich in eine HTML-Datei exportiert wird. Der Standardwert ist false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab) { get; set; } | Gibt an, ob die einzelne Registerkarte exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. Der Standardwert ist „false“. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments) { get; set; } | Gibt an, ob beim Exportieren von Kommentaren beim Speichern der Datei in HTML der Standardwert falsch ist. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink) { get; set; } | Gibt an, ob der vollständige Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung zusammengeführt werden, bevor die Datei gespeichert wird. |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle) { get; set; } | Der Titel der HTML-Seite. Nur zum Speichern im HTML-Stream. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell) { get; set; } | HTML-Tag in Zelle parsen, wie , als Zellenwert oder als HTML-Tag, Standard ist true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference) { get; set; } | Gibt an, ob die HTML- oder MHT-Datei die bevorzugte Präsentation ist. Der Standardwert ist „false“. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache) { get; set; } | Gibt an, ob Diagramm-Cache-Daten aktualisiert werden |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat) { get; } | Ruft das Sicherungsdateiformat ab. |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas) { get; set; } | Gibt an, ob verbundene Zellen validiert werden sollen, bevor die Datei gespeichert wird. |

### Siehe auch

* class [GridSaveOptions](../gridsaveoptions)
* namensraum [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* Montage [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
