---
title: "Klasse HtmlSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlSaveOptions Klasse. Stellt die Optionen zum Speichern einer HTML-Datei dar"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

Stellt die Optionen zum Speichern einer HTML-Datei dar.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/#constructor)() | Erstellt Optionen zum Speichern einer HTML-Datei. |
| [HtmlSaveOptions](htmlsaveoptions/#constructor_1)(SaveFormat) | Erstellt Optionen zum Speichern einer HTM-Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | Gibt an, ob eine generische Schriftart zur CSS‑font-family hinzugefügt werden soll. Der Standardwert ist true |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | Gibt an, ob ein Tooltip‑Text hinzugefügt wird, wenn die Daten nicht vollständig angezeigt werden können. Der Standardwert ist false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur beim Speichern in einen HTML‑Stream. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | Gib das URL-Präfix der angehängten Dateien wie Bilder in der HTML‑Datei an. Nur beim Speichern in einen HTML‑Stream. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Der Ordner für temporäre Dateien, der als Daten-Cache verwendet werden kann.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | Gibt an, ob Formeln vor dem Speichern der HTML‑Datei berechnet werden sollen. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | Liest und setzt das Präfix des CSS‑Namens, der Standardwert ist "". |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | Gibt das Attribut an, das den zu schreibenden Zellnamen kennzeichnet. (z. B. Wenn der Wert "id" ist, wird für die Zelle "A1" die Ausgabe &lt;td id='A1'&gt; sein). Der Standardwert ist null. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Ob Einschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, wird er abgeschnitten.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Leere das Arbeitsbuch nach dem Speichern der Datei.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | Liest oder setzt die zusätzlichen CSS‑Stile für den Formatierer. Funktioniert nur, wenn [`SaveAsSingleFile`](./saveassinglefile/) True ist. CssStyles="body { padding: 5px }"; |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | Stellt den Modus dar, wie DataBar beim Konvertieren von Excel‑Dateien in HTML‑Dateien gerendert wird. Standardwert ist BackgroundColor. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | Gib den Standard‑Schriftartnamen für den Export von HTML an, die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null. |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | Gibt an, ob nur Inline‑Stile angewendet werden, ohne sich auf CSS zu verlassen. Der Standardwert ist false. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | Gibt an, ob Downlevel‑revealed bedingte Kommentare beim Exportieren der Datei nach HTML deaktiviert werden sollen, der Standardwert ist false. |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | Liest oder setzt den Typ der Einbettung von Schriftdateien in die HTML‑Datei. Standardwert ist None, was bedeutet, dass keine Schriftart in HTML eingebettet wird. |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | Optimiere die Ausgabe von HTML durch die Verwendung von CSS‑Custom‑Properties. Zum Beispiel muss bei mehreren Vorkommen desselben Base64‑Bildes das Bilddaten nur einmal gespeichert werden, wodurch die Leistung des resultierenden HTML verbessert wird. Der Standardwert ist false. |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | Gibt an, ob die HTML‑Zeichenentitäten durch Dezimalcodes ersetzt werden. (z. B. "&amp;nbsp;" wird durch "&amp;#160;" ersetzt). Der Standardwert ist false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | Wenn nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | Gibt an, ob ungenutzte Stile ausgeschlossen werden. Bei den erzeugten HTML‑Dateien kann das Ausschließen ungenutzter Stile die Dateigröße verkleinern, ohne die visuellen Effekte zu beeinträchtigen. Daher ist der Standardwert dieser Eigenschaft true. Wenn der Benutzer alle Stile in der Arbeitsmappe für das erzeugte HTML beibehalten muss (z. B. wenn das Arbeitsblatt später aus dem erzeugten HTML wiederhergestellt werden soll), setzen Sie diese Eigenschaft bitte auf false. |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | Gibt an, ob nur das aktive Arbeitsblatt in eine html-Datei exportiert wird. Wenn true, wird nur das aktive Arbeitsblatt in die html-Datei exportiert; wenn false, wird die gesamte Arbeitsmappe in die html-Datei exportiert. Der Standardwert ist false. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | Liest oder setzt den zu exportierenden CellArea des aktuell aktiven Worksheet. Wenn Sie dieses Attribut festlegen, wird der Druckbereich des aktuell aktiven Worksheet weggelassen. Nur der angegebene Bereich wird beim Speichern der Datei als html exportiert. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | Gibt an, ob gefälschte Daten in der unteren Zeile exportiert werden. Der Standardwert ist true. Wenn Sie die html- oder mht-Datei in excel importieren möchten, belassen Sie bitte den Standardwert. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | Gibt an, ob excel-Koordinaten nicht leerer Zellen beim Speichern der Datei als html exportiert werden. Der Standardwert ist false. Wenn Sie das erzeugte html in excel importieren möchten, belassen Sie bitte den Standardwert. |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | Stellt den Typ des Exports von Kommentaren in html-Dateien dar. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | Gibt die Regel für den Export von html-Dateidaten an. Der Standardwert ist All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die html- oder mht-Datei in excel importieren möchten, belassen Sie bitte den Standardwert. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger ist als die maximal anzuzeigende Spalte. Der Standardwert ist false. Wenn Sie die html-Datei in excel importieren möchten, belassen Sie bitte den Standardwert. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | Gibt an, ob Formeln beim Speichern der Datei als html exportiert werden. Der Standardwert ist true. Wenn Sie das erzeugte html in excel importieren möchten, belassen Sie bitte den Standardwert. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | Gibt an, ob Frame‑Skripte und Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die html- oder mht-Datei in excel importieren möchten, belassen Sie bitte den Standardwert. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false. |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML-Dateien exportiert werden. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | Gibt an, ob versteckte Worksheet‑Inhalte exportiert werden. Der Standardwert ist true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | Gibt an, ob Bilder im Base64-Format in html, MHTML oder EPUB gespeichert werden. |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | Gibt an, ob Anker‑Elemente für benannte Bereiche beim Speichern als html exportiert werden. Der Standardwert ist true. |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) Liest oder setzt den ExportObjectListener für den Export von Objekten. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | Gibt an, ob Seitenköpfe exportiert werden. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | Gibt an, ob Seitenköpfe exportiert werden. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | Gibt an, ob nur der Druckbereich in eine html-Datei exportiert wird. Der Standardwert ist false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML-Dateien exportiert werden. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | Gibt an, ob ein ähnlicher Rahmenstil exportiert wird, wenn der Rahmenstil von Browsern nicht unterstützt wird. Wenn Sie die html- oder mht-Datei in excel importieren möchten, belassen Sie bitte den Standardwert. Der Standardwert ist false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | Gibt an, ob das einzelne Registerblatt exportiert wird, wenn die Datei nur ein Worksheet enthält. Der Standardwert ist false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | Gibt an, ob Arbeitsmappeneigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die html- oder mht-Datei in excel importieren möchten, belassen Sie bitte den Standardwert. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | Gibt an, ob das CSS des Worksheets separat exportiert wird. Der Standardwert ist false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | Gibt an, ob Arbeitsblatt‑Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | Ruft den IFilePathProvider ab oder legt ihn fest, um das Arbeitsblatt separat nach HTML zu exportieren. |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | Gibt an, ob die gesamten formatierten Daten einer Zelle angezeigt werden sollen, wenn sie die Spalte überläuft. Wenn true, wird die Spaltenbreite ignoriert und die gesamten Zellen­daten werden exportiert. Wenn false, werden die Daten wie in Excel exportiert. Der Standardwert ist false. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird: Wenn HtmlHiddenColDisplayType "Remove" ist, wird die versteckte Spalte nicht ausgegeben; ist der Wert "Hidden", wird die Spalte ausgegeben, aber verborgen. Der Standardwert ist "Hidden". |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird: Wenn HtmlHiddenRowDisplayType "Remove" ist, wird die versteckte Zeile nicht ausgegeben; ist der Wert "Hidden", wird die Zeile ausgegeben, aber verborgen. Der Standardwert ist "Hidden". |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | Gibt an, ob überlaufender Text ausgeblendet werden soll, wenn das Zellenformat auf Zeilenumbruch gesetzt ist. Der Standardwert ist false. |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | Gibt an, ob ein über mehrere Zellen erstreckender Text beim Speichern einer Excel‑Datei im HTML‑Format auf dieselbe Weise wie MS Excel angezeigt wird. Standardmäßig ist der Wert Default, sodass bei übergreifenden Zeichenketten nur geringe Unterschiede zwischen den von Aspose.Cells und MS Excel erzeugten HTML‑Dateien bestehen. Für die Erstellung großer HTML‑Dateien ist die Leistung jedoch mehrere Male höher, wenn der Wert auf Cross gesetzt wird, im Vergleich zu Default oder Fit2Cell. |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | Gibt die HTML‑Standardversion an, die beim Speichern im HTML‑Format verwendet werden soll. Der Standardwert ist HtmlVersion.Default. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | Gibt an, ob nicht sichtbare Formen exportiert werden sollen. |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | Rufen Sie das ImageOrPrintOptions‑Objekt vor dem Exportieren ab. |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. Der Standardwert ist true. |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | Gibt an, ob Tabellenränder zusammengeführt werden. Der Standardwert ist true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. Nur beim Speichern in einen HTML‑Stream. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | Gibt an, ob Kommentare beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | Gibt an, ob ein Vollpfad‑Link in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false. |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | Gibt an, ob das ausgegebene HTML mit dem IE‑Browser kompatibel ist. Der Standardwert ist false. |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | Gibt an, ob JavaScript mit Browsern kompatibel ist, die kein JavaScript unterstützen. Der Standardwert ist true. |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | Gibt an, ob das ausgegebene HTML mit mobilen Geräten kompatibel ist. Der Standardwert ist false. |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | Ruft den Layoutmodus ab oder legt ihn fest, wenn in HTML gespeichert wird. Der Standardwert ist Normal. |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | Gibt den Typ des target‑Attributs in einem `<a>`‑Link an. Der Standardwert ist HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) Gibt an, ob leere TD-Elemente beim Exportieren der Datei nach HTML zwangsweise zusammengeführt werden. Die Größe der HTML-Datei wird nach Einstellung des Werts auf true deutlich reduziert. Der Standardwert ist false. Wenn Sie die HTML-Datei nach Excel importieren oder beim Speichern der Datei nach HTML perfekte Rasterlinien exportieren möchten, belassen Sie bitte den Standardwert. |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | Die Option, zusammenhängende leere Zellen (leere td-Elemente) zusammenzuführen. Der Standardwert ist MergeEmptyTdType.Default. |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | Gibt an, wie OfficeMath-Objekte nach HTML exportiert werden. Der Standardwert ist Image. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | Der Titel der HTML-Seite. Nur beim Speichern in einen HTML-Stream. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | Gibt an, ob HTML‑Tags (wie `<div></div>`) in einer Zelle als Zellenwert geparst oder unverändert beibehalten werden sollen. Der Standardwert ist true. |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | Gibt an, ob HTML‑ oder MHT‑Datei die Präsentationspräferenz ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung erhalten möchten, setzen Sie den Wert bitte auf true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | Gibt an, ob die HTML als einzelne Datei gespeichert wird. Der Standardwert ist false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Liest das Speicherdateiformat.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | Liest oder setzt die zu rendernden Arbeitsblätter. Standard ist alle sichtbaren Arbeitsblätter in der Arbeitsmappe: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | Gibt an, ob beim Speichern als einzelne HTML‑Datei alle Arbeitsblätter angezeigt werden. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | Gibt an, wie Leerzeichen in der HTML‑Ausgabe gerendert werden. Diese Option wird derzeit nur auf numerische Formate (z. B. Buchhaltungsformat) angewendet. Der Standardwert ist Css. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | Liest oder setzt den IStreamProvider für den Export von Objekten. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | Liest und setzt das Präfix des CSS‑Typs, wie tr, col, td usw., die im Table‑Element enthalten sind, das das spezifische TableCssId‑Attribut besitzt. Der Standardwert ist \"\". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. Der Standardwert ist false.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Liest oder setzt den Warnungs-Callback.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | Gibt an, ob die Spaltenbreite in Skalierungseinheiten nach HTML exportiert wird. Der Standardwert ist false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | Gibt an, ob beim Speichern der Datei nach HTML über die Arbeitsblatt‑Zoomstufe in die HTML gezoomt wird. Der Standardwert ist false. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsDemo
    {
        public static void HtmlSaveOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Erstelle eine Instanz von HtmlSaveOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IgnoreInvisibleShapes = true,
                PageTitle = "Sample HTML Page",
                AttachedFilesDirectory = "attached_files",
                AttachedFilesUrlPrefix = "http://example.com/files/",
                DefaultFontName = "Arial",
                AddGenericFont = true,
                WorksheetScalable = false,
                IsExportComments = false,
                ExportCommentsType = PrintCommentsType.PrintNoComments,
                DisableDownlevelRevealedComments = false,
                IsExpImageToTempDir = false,
                ImageScalable = true,
                WidthScalable = false,
                ExportSingleTab = false,
                ExportImagesAsBase64 = false,
                ExportActiveWorksheetOnly = false,
                ExportPrintAreaOnly = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 },
                ParseHtmlTagInCell = true,
                HtmlCrossStringType = HtmlCrossType.Default,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden,
                Encoding = System.Text.Encoding.UTF8,
                SaveAsSingleFile = false,
                ShowAllSheets = false,
                ExportPageHeaders = false,
                ExportPageFooters = false,
                ExportHiddenWorksheet = true,
                PresentationPreference = false,
                CellCssPrefix = "",
                TableCssId = "",
                IsFullPathLink = false,
                ExportWorksheetCSSSeparately = false,
                ExportSimilarBorderStyle = false,
                MergeEmptyTdForcely = false,
                MergeEmptyTdType = MergeEmptyTdType.Default,
                ExportCellCoordinate = false,
                ExportExtraHeadings = false,
                ExportHeadings = false,
                ExportRowColumnHeadings = false,
                ExportFormula = true,
                AddTooltipText = false,
                ExportGridLines = false,
                ExportBogusRowData = true,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = true,
                ExportWorksheetProperties = true,
                ExportWorkbookProperties = true,
                ExportFrameScriptsAndProperties = true,
                ExportDataOptions = HtmlExportDataOptions.All,
                LinkTargetType = HtmlLinkTargetType.Parent,
                IsIECompatible = false,
                FormatDataIgnoreColumnWidth = false,
                CalculateFormula = true,
                IsJsBrowserCompatible = true,
                IsMobileCompatible = false,
                CssStyles = "body { padding: 5px }",
                HideOverflowWrappedText = false,
                IsBorderCollapsed = true,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Speichere die Arbeitsmappe als HTML
            workbook.Save("HtmlSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


