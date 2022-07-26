---
title: HtmlSaveOptions
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert die Optionen zum Speichern der HTML-Datei.
type: docs
weight: 3740
url: /de/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Repräsentiert die Optionen zum Speichern der HTML-Datei.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions#constructor)() | Erstellt Optionen zum Speichern der HTML-Datei. |
| [HtmlSaveOptions](htmlsaveoptions#constructor_1)(SaveFormat) | Erstellt Optionen zum Speichern der HTML-Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext) { get; set; } | Gibt an, ob QuickInfo-Text hinzugefügt wird, wenn die Daten nicht vollständig angezeigt werden können. Der Standardwert ist „false“. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory) { get; set; } | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur zum Speichern im HTML-Stream. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix) { get; set; } | Geben Sie das URL-Präfix von angehängten Dateien wie Bild in der HTML-Datei an. Nur zum Speichern im HTML-Stream. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Der zwischengespeicherte Dateiordner wird verwendet, um einige große Daten zu speichern. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix) { get; set; } | Ruft das Präfix des CSS-Namens ab und legt es fest, der Standardwert ist "". |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Machen Sie die Arbeitsmappe nach dem Speichern der Datei leer. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis automatisch erstellt, bevor die Datei gespeichert wird. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname) { get; set; } | Geben Sie den Namen der Standardschriftart zum Exportieren von HTML an, die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist, Wenn diese Eigenschaft null ist, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat, der Standardwert ist null. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments) { get; set; } | Gibt an, ob beim Exportieren der Datei in HTML bedingte Kommentare auf niedrigerer Ebene deaktiviert werden sollen. Der Standardwert ist „false“. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding) { get; set; } | Wenn nicht festgelegt, verwenden Sie Encoding.UTF8 als Standardcodierungstyp. |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles) { get; set; } | Gibt an, ob nicht verwendete Stile ausgeschlossen werden. Bei den generierten HTML-Dateien kann das Ausschließen nicht verwendeter Stile die Dateigröße verkleinern , ohne die visuellen Effekte zu beeinträchtigen. Der Standardwert dieser Eigenschaft ist also true. Wenn der Benutzer alle Stile in der Arbeitsmappe für das generierte HTML beibehalten muss (z. B. das Szenario, dass user die Arbeitsmappe später aus dem generierten HTML wiederherstellen muss), setzen Sie diese Eigenschaft bitte auf false . |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly) { get; set; } | Gibt an, ob die gesamte Arbeitsmappe in eine HTML-Datei exportiert wird. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea) { get; set; } | Ermittelt oder setzt den exportierenden CellArea des aktuell aktiven Arbeitsblatts. Wenn Sie dieses Attribut setzen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen. Nur der angegebene Bereich wird exportiert, wenn die Datei in HTML gespeichert wird. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata) { get; set; } | Gibt an, ob falsche Daten in der unteren Zeile exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate) { get; set; } | Gibt an, ob beim Speichern der Datei in HTML Excel-Koordinaten von nicht leeren Zellen exportiert werden. Der Standardwert ist false. Wenn Sie die HTML-Ausgabe in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions) { get; set; } | Gibt die Regel zum Exportieren von HTML-Dateidaten an. Der Standardwert ist Alle. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties) { get; set; } | Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist wahr. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings) { get; set; } | Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger als die maximale Anzeigespalte ist. Der Standardwert ist „false“. Wenn Sie die HTML-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula) { get; set; } | Gibt an, ob die Formel beim Speichern der Datei in HTML exportiert wird. Der Standardwert ist true. Wenn Sie die HTML-Ausgabe in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties) { get; set; } | Gibt an, ob Rahmenskripte und Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines) { get; set; } | Gibt an, ob die Gitternetzlinien exportiert werden. Der Standardwert ist „false“. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet) { get; set; } | Gibt an, ob der Inhalt des ausgeblendeten Arbeitsblatts exportiert wird. Der Standardwert ist wahr. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64) { get; set; } | Gibt an, ob Bilder im Base64-Format in HTML, MHTML oder EPUB gespeichert werden. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters) { get; set; } | Gibt an, ob Seitenkopfzeilen exportiert werden. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders) { get; set; } | Gibt an, ob Seitenkopfzeilen exportiert werden. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly) { get; set; } | Gibt an, ob nur der Druckbereich in eine HTML-Datei exportiert wird. Der Standardwert ist false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings) { get; set; } | Gibt an, ob beim Speichern in HTML-Dateien die Zeilen- und Spaltenüberschriften des Blatts exportiert werden. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle) { get; set; } | Gibt an, ob der ähnliche Rahmenstil exportiert wird, wenn der Rahmenstil nicht von Browsern unterstützt wird. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. Der Standardwert ist „false“. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab) { get; set; } | Gibt an, ob die einzelne Registerkarte exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. Der Standardwert ist „false“. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties) { get; set; } | Gibt an, ob Arbeitsmappeneigenschaften exportiert werden. Der Standardwert ist wahr. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately) { get; set; } | Gibt an, ob das Arbeitsblatt-CSS separat exportiert werden soll. Der Standardwert ist „false“. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties) { get; set; } | Gibt an, ob Arbeitsblatteigenschaften exportiert werden. Der Standardwert ist wahr. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider) { get; set; } | Ruft den IFilePathProvider für den separaten Export von Arbeitsblättern in HTML ab oder legt ihn fest. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype) { get; set; } | Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel, bevor Sie diese im HTML-Format speichern, wenn HtmlHiddenColDisplayType "Remove" ist, würde die versteckte Spalte nicht ausgegeben, wenn der Wert "Hidden" ist, würde die Spalte ausgegeben, aber ausgeblendet wurde, ist der Standardwert „Ausgeblendet“ |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype) { get; set; } | Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor Sie diese im HTML-Format speichern, wenn HtmlHiddenRowDisplayType "Remove" ist, würde die versteckte Zeile nicht ausgegeben, wenn der Wert "Hidden" ist, würde die Zeile ausgegeben, aber ausgeblendet wurde, ist der Standardwert „Ausgeblendet“ |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype) { get; set; } | Gibt an, ob eine zellenübergreifende Zeichenfolge beim Speichern einer Excel-Datei im HTML-Format auf die gleiche Weise wie MS Excel angezeigt wird. Standardmäßig ist der Wert Standard, daher gibt es bei zellenübergreifenden Zeichenfolgen kaum einen Unterschied zwischen HTML von Aspose.Cells und MS Excel erstellte Dateien. Aber die Leistung beim Erstellen großer HTML-Dateien, wenn der Wert auf Cross gesetzt wird, wäre um ein Vielfaches schneller als die Einstellung auf Default oder Fit2Cell. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes) { get; set; } | Geben Sie an, ob diese nicht sichtbaren Formen exportiert werden |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions) { get; } | Rufen Sie das ImageOrPrintOptions-Objekt ab, bevor Sie exportieren |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable) { get; set; } | Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. Der Standardwert ist wahr. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir) { get; set; } | Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. Nur zum Speichern im HTML-Stream. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments) { get; set; } | Gibt an, ob beim Exportieren von Kommentaren beim Speichern der Datei in HTML der Standardwert falsch ist. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink) { get; set; } | Gibt an, ob der vollständige Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false. |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype) { get; set; } | Gibt den Typ des Zielattributs im Link &lt;a&gt; an. Der Standardwert ist HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung zusammengeführt werden, bevor die Datei gespeichert wird. |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely) { get; set; } | Gibt an, ob leere TD-Elemente beim Exportieren der Datei in HTML zwangsweise zusammengeführt werden. Die Größe der HTML-Datei wird erheblich reduziert, nachdem der Wert auf true gesetzt wurde. Der Standardwert ist falsch. Wenn Sie die HTML-Datei in Excel importieren oder beim Speichern der Datei in HTML perfekte Gitterlinien exportieren möchten, behalten Sie bitte den Standardwert bei. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle) { get; set; } | Der Titel der HTML-Seite. Nur zum Speichern im HTML-Stream. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell) { get; set; } | HTML-Tag in Zelle parsen, wie , als Zellenwert oder als HTML-Tag, Standard ist true |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference) { get; set; } | Gibt an, ob die HTML- oder MHT-Datei die bevorzugte Präsentation ist. Der Standardwert ist „false“. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Gibt an, ob Diagramm-Cache-Daten aktualisiert werden |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile) { get; set; } | Gibt an, ob die HTML-Datei als einzelne Datei gespeichert wird. Der Standardwert ist „false“. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Ruft das Sicherungsdateiformat ab. |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets) { get; set; } | Gibt an, ob beim Speichern als einzelne HTML-Datei alle Blätter angezeigt werden. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Gibt an, ob extern definierte Namen vor dem Speichern der Datei sortiert werden. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider) { get; set; } | Ruft den IStreamProvider zum Exportieren von Objekten ab oder setzt ihn. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid) { get; set; } | Erhält und setzt das Präfix des Typs CSS-Namen wie tr, col, td usw. Sie sind im Tabellenelement enthalten, das das spezifische Attribut TableCssId hat. Der Standardwert ist "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Gibt an, ob die SmartArt-Einstellung aktualisiert wird. Der Standardwert ist „false“. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Gibt an, ob verbundene Zellen validiert werden sollen, bevor die Datei gespeichert wird. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Ruft Warnrückruf ab oder legt ihn fest. |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable) { get; set; } | Gibt an, ob eine skalierbare Einheit verwendet wird, um die Spaltenbreite beim Exportieren der Datei in HTML zu beschreiben. Der Standardwert ist „false“. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable) { get; set; } | Gibt an, ob das HTML über die Zoomstufe des Arbeitsblatts vergrößert oder verkleinert wird, wenn die Datei in HTML gespeichert wird. Der Standardwert ist „false“. |

### Siehe auch

* class [SaveOptions](../saveoptions)
* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
