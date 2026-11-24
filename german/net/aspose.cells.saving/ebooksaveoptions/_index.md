---
title: "Klasse EbookSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Saving.EbookSaveOptions Klasse. Stellt die Optionen zum Speichern von E‑Book‑Dateien dar"
type: docs
url: /de/net/aspose.cells.saving/ebooksaveoptions/
---
## EbookSaveOptions class

Stellt die Optionen zum Speichern der ebook-Datei dar.

```csharp
public class EbookSaveOptions : HtmlSaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [EbookSaveOptions](ebooksaveoptions/#constructor)() | Erstellt Optionen zum Speichern von E‑Book‑Dateien. |
| [EbookSaveOptions](ebooksaveoptions/#constructor_1)(SaveFormat) | Erstellt Optionen zum Speichern von E‑Book‑Dateien. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Gibt an, ob eine generische Schriftart zur CSS‑font-family hinzugefügt werden soll. Der Standardwert ist true (geerbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Gibt an, ob ein Tooltip‑Text hinzugefügt wird, wenn die Daten nicht vollständig angezeigt werden können. Der Standardwert ist false (geerbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur beim Speichern in einen HTML‑Stream (geerbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Geben Sie das URL‑Präfix für angehängte Dateien wie Bilder in der HTML‑Datei an. Nur beim Speichern in einen HTML‑Stream (geerbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Der Ordner für temporäre Dateien, die als Daten‑Cache verwendet werden können (geerbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Gibt an, ob Formeln vor dem Speichern der HTML‑Datei berechnet werden sollen (geerbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Liest und setzt das Präfix des CSS‑Namens, der Standardwert ist "" (geerbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Gibt das Attribut an, das den zu schreibenden Zellnamen angibt. (z. B. Wenn der Wert \"id\" ist, wird für die Zelle \"A1\" die Ausgabe &lt;td id='A1'&gt; sein). Der Standardwert ist null (geerbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Ob Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB eingeben, wird er abgeschnitten (geerbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Leert die Arbeitsmappe nach dem Speichern der Datei (geerbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt (geerbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Liest oder setzt die zusätzlichen CSS‑Stile für den Formatter. Funktioniert nur, wenn [`SaveAsSingleFile`](../../aspose.cells/htmlsaveoptions/saveassinglefile/) true ist. CssStyles=\"body { padding: 5px }\" (geerbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Stellt den Modus dar, wie DataBar beim Konvertieren von Excel‑Dateien in HTML‑Dateien gerendert wird. Der Standardwert ist BackgroundColor (geerbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Geben Sie den Standard‑Schriftartnamen für den Export nach HTML an, die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat; der Standardwert ist null (geerbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Gibt an, ob nur Inline‑Stile angewendet werden, ohne sich auf CSS zu verlassen. Der Standardwert ist false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Gibt an, ob Downlevel‑revealed bedingte Kommentare beim Exportieren der Datei nach HTML deaktiviert werden, der Standardwert ist false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Liest oder legt den Typ der Einbettung von Schriftdateien in die HTML‑Datei fest. Der Standardwert ist None, was bedeutet, dass keine Schrift in HTML eingebettet wird.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Optimiert die Ausgabe von HTML durch die Verwendung von CSS‑benutzerdefinierten Eigenschaften. Zum Beispiel, wenn es mehrere Vorkommen eines Base64‑Bildes gibt, muss mit einer benutzerdefinierten Eigenschaft die Bilddaten nur einmal gespeichert werden, sodass die Leistung des resultierenden HTML verbessert werden kann. Der Standardwert ist false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Gibt an, ob die HTML‑Zeichenentitäten durch dezimale Codes ersetzt werden. (z. B. \"&amp;nbsp;\" wird durch \"&amp;#160;\" ersetzt). Der Standardwert ist false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Wenn nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls‑Datei verschlüsselt werden. Der Standardwert ist true.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Gibt an, ob ungenutzte Stile ausgeschlossen werden. Für die erzeugten HTML‑Dateien kann das Ausschließen ungenutzter Stile die Dateigröße verkleinern, ohne die visuellen Effekte zu beeinträchtigen. Daher ist der Standardwert dieser Eigenschaft true. Wenn der Benutzer alle Stile in der Arbeitsmappe für das erzeugte HTML beibehalten muss (z. B. wenn die Arbeitsmappe später aus dem erzeugten HTML wiederhergestellt werden soll), setzen Sie diese Eigenschaft bitte auf false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Gibt an, ob nur das aktive Arbeitsblatt in eine HTML‑Datei exportiert wird. Wenn true, wird nur das aktive Arbeitsblatt in die HTML‑Datei exportiert; wenn false, wird die gesamte Arbeitsmappe in die HTML‑Datei exportiert. Der Standardwert ist false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Liest oder legt den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts fest. Wenn Sie dieses Attribut setzen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen. Nur der angegebene Bereich wird beim Speichern der Datei nach HTML exportiert.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Gibt an, ob fehlerhafte Daten der unteren Zeile exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Gibt an, ob beim Speichern der Datei als HTML die Excel‑Koordinaten nicht leerer Zellen exportiert werden. Der Standardwert ist false. Wenn Sie das erzeugte HTML nach Excel importieren möchten, behalten Sie bitte den Standardwert bei. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Stellt den Typ des Exports von Kommentaren in HTML-Dateien dar. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Gibt die Regel für den Export von HTML-Dateidaten an. Der Standardwert ist All. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger ist als die maximale Anzeigespalte. Der Standardwert ist false. Wenn Sie die HTML-Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Gibt an, ob Formeln beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist true. Wenn Sie das erzeugte HTML nach Excel importieren möchten, behalten Sie bitte den Standardwert bei. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Gibt an, ob Frame‑Skripte und Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Gibt an, ob beim Speichern in HTML-Dateien die Zeilen‑ und Spaltenüberschriften des Blatts exportiert werden. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Gibt an, ob der Inhalt ausgeblendeter Arbeitsblätter exportiert wird. Der Standardwert ist true. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Gibt an, ob Bilder im Base64-Format in HTML, MHTML oder EPUB gespeichert werden. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Gibt an, ob Ankerelemente für benannte Bereiche beim Speichern als HTML exportiert werden. Der Standardwert ist true. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Ruft den ExportObjectListener für den Export von Objekten ab oder legt ihn fest. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Gibt an, ob Seitenkopfzeilen exportiert werden. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Gibt an, ob Seitenkopfzeilen exportiert werden. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Gibt an, ob nur der Druckbereich in die HTML-Datei exportiert wird. Der Standardwert ist false. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Gibt an, ob beim Speichern in HTML-Dateien die Zeilen‑ und Spaltenüberschriften des Blatts exportiert werden. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Gibt an, ob beim Exportieren ein ähnlicher Rahmenstil verwendet wird, wenn der Rahmenstil von Browsern nicht unterstützt wird. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. Der Standardwert ist false. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Gibt an, ob beim Exportieren ein einzelner Tab verwendet wird, wenn die Datei nur ein Arbeitsblatt enthält. Der Standardwert ist false. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Gibt an, ob Arbeitsmappen‑Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Gibt an, ob das Arbeitsblatt‑CSS separat exportiert wird. Der Standardwert ist false. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Gibt an, ob Arbeitsblatt‑Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Liest oder setzt den IFilePathProvider für den separaten Export von Arbeitsblättern nach HTML. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Gibt an, ob die vollständig formatierte Zellen­daten angezeigt werden, wenn sie die Spalte überlaufen. Wenn true, wird die Spaltenbreite ignoriert und die gesamten Zellen­daten werden exportiert. Wenn false, werden die Daten wie in Excel exportiert. Der Standardwert ist false. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird: Wenn HtmlHiddenColDisplayType "Remove" ist, wird die versteckte Spalte nicht ausgegeben; ist der Wert "Hidden", wird die Spalte ausgegeben, aber verborgen. Der Standardwert ist "Hidden". (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird: Wenn HtmlHiddenRowDisplayType "Remove" ist, wird die versteckte Zeile nicht ausgegeben; ist der Wert "Hidden", wird die Zeile ausgegeben, aber verborgen. Der Standardwert ist "Hidden". (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Gibt an, ob überlaufender Text ausgeblendet wird, wenn das Zellenformat auf Zeilenumbruch gesetzt ist. Der Standardwert ist false. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Gibt an, ob ein über mehrere Zellen erstreckender Text beim Speichern einer Excel‑Datei im HTML‑Format genauso wie in MS Excel angezeigt wird. Standardmäßig ist der Wert Default, sodass es bei über Zellen erstreckenden Texten kaum Unterschiede zwischen den von Aspose.Cells und MS Excel erzeugten HTML‑Dateien gibt. Bei der Erstellung großer HTML‑Dateien ist die Leistung jedoch mehrere Male höher, wenn der Wert auf Cross gesetzt wird, im Vergleich zu Default oder Fit2Cell. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Gibt die Version des HTML-Standards an, die beim Speichern des HTML-Formats verwendet werden soll. Der Standardwert ist HtmlVersion.Default.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Gibt an, ob nicht sichtbare Formen exportiert werden sollen(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Rufen Sie das ImageOrPrintOptions-Objekt vor dem Exportieren ab(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. Der Standardwert ist true.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Gibt an, ob die Tabellenränder zusammengeführt werden. Der Standardwert ist true.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. Nur beim Speichern in einen HTML‑Stream.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Gibt an, ob Kommentare beim Speichern der Datei als HTML exportiert werden, der Standardwert ist false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Gibt an, ob ein vollständiger Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Gibt an, ob das ausgegebene HTML mit dem IE‑Browser kompatibel ist. Der Standardwert ist false(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Gibt an, ob JavaScript mit Browsern kompatibel ist, die JavaScript nicht unterstützen. Der Standardwert ist true.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Gibt an, ob das ausgegebene HTML mit mobilen Geräten kompatibel ist. Der Standardwert ist false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Ruft den Layoutmodus beim Speichern als HTML ab oder legt ihn fest. Der Standardwert ist Normal(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Gibt den Typ des target-Attributs in einem `<a>`‑Link an. Der Standardwert ist HtmlLinkTargetType.Parent.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Gibt an, ob leere TD‑Elemente beim Exportieren der Datei nach HTML zwangsweise zusammengeführt werden. Die Größe der HTML‑Datei wird nach dem Setzen des Werts auf true deutlich reduziert. Der Standardwert ist false. Wenn Sie die HTML‑Datei nach Excel importieren oder beim Speichern der Datei nach HTML perfekte Rasterlinien exportieren möchten, behalten Sie bitte den Standardwert bei.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | Die Option, zusammenhängende leere Zellen (leere td‑Elemente) zusammenzuführen. Der Standardwert ist MergeEmptyTdType.Default.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Gibt an, wie OfficeMath-Objekte nach HTML exportiert werden, Standardwert ist Image.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | Der Titel der html-Seite. Nur zum Speichern in html-Stream.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Gibt an, ob html-Tag(such as `<div></div>`) in einer Zelle als Zellenwert geparst oder unverändert beibehalten werden soll. Der Standardwert ist true.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Gibt an, ob html- oder mht-Datei die Präsentationspräferenz ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung erhalten möchten, setzen Sie den Wert auf true.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Gibt an, ob die neuesten Daten des Diagramms zwischengespeichert werden sollen.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Gibt an, ob das html als einzelne Datei gespeichert wird. Der Standardwert ist false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ermittelt das Speicherdateiformat.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Ermittelt oder legt die zu rendernden Arbeitsblätter fest. Standard ist alle sichtbaren Arbeitsblätter in der Arbeitsmappe: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Gibt an, ob beim Speichern als einzelne html-Datei alle Arbeitsblätter angezeigt werden.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Gibt an, wie Leerzeichen in der HTML-Ausgabe gerendert werden. Diese Option wird derzeit nur auf numerische Formate (z. B. Buchhaltungsformat) angewendet. Der Standardwert ist Css.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Ermittelt oder legt den IStreamProvider für den Export von Objekten fest.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Ermittelt und legt das Präfix des CSS-Typsnamens wie tr, col, td usw. fest, die im Table-Element enthalten sind, das das spezifische TableCssId-Attribut besitzt. Der Standardwert ist "".(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Gibt an, ob die SmartArt-Einstellung aktualisiert wird. Der Standardwert ist false.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ermittelt oder legt den Warnungs-Callback fest.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Gibt an, ob die Spaltenbreite in Skalierungseinheiten nach html exportiert wird. Der Standardwert ist false.(Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Gibt an, ob beim Speichern der Datei als HTML das HTML über die Arbeitsblatt-Zoomstufe vergrößert oder verkleinert wird, der Standardwert ist false. (Vererbt von [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsDemo
    {
        public static void EbookSaveOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello World");

            // Erstelle eine Instanz von EbookSaveOptions
            EbookSaveOptions saveOptions = new EbookSaveOptions();

            // Eigenschaften festlegen
            saveOptions.IgnoreInvisibleShapes = true;
            saveOptions.PageTitle = "Sample Page Title";
            saveOptions.AttachedFilesDirectory = "attached_files";
            saveOptions.AttachedFilesUrlPrefix = "http://example.com/files/";
            saveOptions.DefaultFontName = "Arial";
            saveOptions.AddGenericFont = true;
            saveOptions.WorksheetScalable = false;
            saveOptions.IsExportComments = false;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintNoComments;
            saveOptions.DisableDownlevelRevealedComments = false;
            saveOptions.IsExpImageToTempDir = false;
            saveOptions.ImageScalable = true;
            saveOptions.WidthScalable = false;
            saveOptions.ExportSingleTab = false;
            saveOptions.ExportImagesAsBase64 = false;
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportPrintAreaOnly = false;
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.Encoding = System.Text.Encoding.UTF8;
            saveOptions.SaveAsSingleFile = false;
            saveOptions.ShowAllSheets = true;
            saveOptions.ExportPageHeaders = true;
            saveOptions.ExportPageFooters = true;
            saveOptions.ExportHiddenWorksheet = true;
            saveOptions.PresentationPreference = false;
            saveOptions.CellCssPrefix = "cell_";
            saveOptions.TableCssId = "table_";
            saveOptions.IsFullPathLink = false;
            saveOptions.ExportWorksheetCSSSeparately = false;
            saveOptions.ExportSimilarBorderStyle = false;
            saveOptions.MergeEmptyTdForcely = false;
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.Default;
            saveOptions.ExportCellCoordinate = false;
            saveOptions.ExportExtraHeadings = false;
            saveOptions.ExportHeadings = true;
            saveOptions.ExportRowColumnHeadings = true;
            saveOptions.ExportFormula = true;
            saveOptions.AddTooltipText = false;
            saveOptions.ExportGridLines = false;
            saveOptions.ExportBogusRowData = true;
            saveOptions.ExcludeUnusedStyles = true;
            saveOptions.ExportDocumentProperties = true;
            saveOptions.ExportWorksheetProperties = true;
            saveOptions.ExportWorkbookProperties = true;
            saveOptions.ExportFrameScriptsAndProperties = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Parent;
            saveOptions.IsIECompatible = false;
            saveOptions.FormatDataIgnoreColumnWidth = false;
            saveOptions.CalculateFormula = true;
            saveOptions.IsJsBrowserCompatible = true;
            saveOptions.IsMobileCompatible = false;
            saveOptions.CssStyles = "body { padding: 5px }";
            saveOptions.HideOverflowWrappedText = false;
            saveOptions.IsBorderCollapsed = true;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = "cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.WarningCallback = null;
            saveOptions.UpdateSmartArt = true;

            // Speichere die Arbeitsmappe in einer HTML-Datei mit den angegebenen Optionen
            workbook.Save("EbookSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../../aspose.cells/htmlsaveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


