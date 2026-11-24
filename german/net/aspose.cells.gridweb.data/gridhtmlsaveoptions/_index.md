---
title: "Klasse GridHtmlSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.GridHtmlSaveOptions-Klasse. Stellt die Optionen zum Speichern einer HTML-Datei dar"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridhtmlsaveoptions/
---
## GridHtmlSaveOptions class

Stellt die Optionen zum Speichern einer HTML-Datei dar.

```csharp
public class GridHtmlSaveOptions : GridSaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor)() | Erstellt Optionen zum Speichern einer HTML-Datei. |
| [GridHtmlSaveOptions](gridhtmlsaveoptions/#constructor_1)(GridSaveFormat) | Erstellt Optionen zum Speichern einer HTM-Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesdirectory/) { get; set; } | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur beim Speichern in einen HTML‑Stream. |
| [AttachedFilesUrlPrefix](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Gib das URL-Präfix der angehängten Dateien wie Bilder in der HTML‑Datei an. Nur beim Speichern in einen HTML‑Stream. |
| [CachedFileFolder](../../aspose.cells.gridweb.data/gridsaveoptions/cachedfilefolder/) { get; set; } | Der Zwischenspeicherordner wird verwendet, um einige große Daten zu speichern. (Vererbt von [`GridSaveOptions`](../gridsaveoptions/).) |
| [ClearData](../../aspose.cells.gridweb.data/gridsaveoptions/cleardata/) { get; set; } | Leert die Arbeitsmappe nach dem Speichern der Datei. (Vererbt von [`GridSaveOptions`](../gridsaveoptions/).) |
| [CreateDirectory](../../aspose.cells.gridweb.data/gridsaveoptions/createdirectory/) { get; set; } | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. (Vererbt von [`GridSaveOptions`](../gridsaveoptions/).) |
| [DefaultFontName](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/defaultfontname/) { get; set; } | Gib den Standard‑Schriftartnamen für den Export von HTML an, die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null. |
| [Encoding](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/encoding/) { get; set; } | Wenn nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet. |
| [ExportActiveWorksheetOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Gibt an, ob die gesamte Arbeitsmappe in eine HTML-Datei exportiert wird. |
| [ExportArea](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportarea/) { get; set; } | Liest oder setzt den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts. Wenn Sie dieses Attribut setzen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen. Nur der angegebene Bereich wird beim Speichern der Datei als HTML exportiert. |
| [ExportGridLines](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportgridlines/) { get; set; } | Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false. |
| [ExportHeadings](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportheadings/) { get; set; } | Gibt an, ob Überschriften beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist false. Wenn Sie die HTML-Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [ExportHiddenWorksheet](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exporthiddenworksheet/) { get; set; } | Gibt an, ob versteckte Worksheet‑Inhalte exportiert werden. Der Standardwert ist true. |
| [ExportImagesAsBase64](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportimagesasbase64/) { get; set; } | Gibt an, ob Bilder im Base64-Format in html, MHTML oder EPUB gespeichert werden. |
| [ExportPrintAreaOnly](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportprintareaonly/) { get; set; } | Gibt an, ob nur der Druckbereich in eine html-Datei exportiert wird. Der Standardwert ist false. |
| [ExportSingleTab](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/exportsingletab/) { get; set; } | Gibt an, ob das einzelne Registerblatt exportiert wird, wenn die Datei nur ein Worksheet enthält. Der Standardwert ist false. |
| [IsExportComments](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isexportcomments/) { get; set; } | Gibt an, ob Kommentare beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist false. |
| [IsFullPathLink](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/isfullpathlink/) { get; set; } | Gibt an, ob ein Vollpfad‑Link in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false. |
| [MergeAreas](../../aspose.cells.gridweb.data/gridsaveoptions/mergeareas/) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. (Vererbt von [`GridSaveOptions`](../gridsaveoptions/).) |
| [PageTitle](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/pagetitle/) { get; set; } | Der Titel der HTML-Seite. Nur beim Speichern in einen HTML-Stream. |
| [ParseHtmlTagInCell](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/parsehtmltagincell/) { get; set; } | Parsen von HTML-Tags in Zellen, wie , als Zellenwert oder als HTML-Tag, Standard ist true |
| [PresentationPreference](../../aspose.cells.gridweb.data/gridhtmlsaveoptions/presentationpreference/) { get; set; } | Gibt an, ob HTML- oder MHT-Datei die bevorzugte Darstellung ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung erhalten möchten, setzen Sie den Wert bitte auf true. |
| [RefreshChartCache](../../aspose.cells.gridweb.data/gridsaveoptions/refreshchartcache/) { get; set; } | Gibt an, ob Diagramm-Cache-Daten aktualisiert werden (Vererbt von [`GridSaveOptions`](../gridsaveoptions/).) |
| [SaveFormat](../../aspose.cells.gridweb.data/gridsaveoptions/saveformat/) { get; } | Liest das Speicherformat der Datei. (Vererbt von [`GridSaveOptions`](../gridsaveoptions/).) |
| [SortNames](../../aspose.cells.gridweb.data/gridsaveoptions/sortnames/) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. (Vererbt von [`GridSaveOptions`](../gridsaveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells.gridweb.data/gridsaveoptions/validatemergedareas/) { get; set; } | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. (Vererbt von [`GridSaveOptions`](../gridsaveoptions/).) |

### Siehe auch

* class [GridSaveOptions](../gridsaveoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


