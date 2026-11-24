---
title: "Klasse PptxSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PptxSaveOptions‑Klasse. Repräsentiert die PPTX‑Speicheroptionen"
type: docs
url: /de/net/aspose.cells/pptxsaveoptions/
---
## PptxSaveOptions class

Stellt die pptx-Speicheroptionen dar.

```csharp
public class PptxSaveOptions : PaginatedSaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PptxSaveOptions](pptxsaveoptions/#constructor)() | Stellt die pptx-Speicheroptionen dar. |
| [PptxSaveOptions](pptxsaveoptions/#constructor_1)(bool) | Repräsentiert Optionen zum Speichern einer .pptx‑Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AdjustFontSizeForRowType](../../aspose.cells/pptxsaveoptions/adjustfontsizeforrowtype/) { get; set; } | Gibt an, welche Art von Linie die Schriftgröße anpassen muss, wenn die Zeilenhöhe klein ist. |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße der Seiten­einrichtung wird ignoriert, und die anderen Einstellungen der Seiten­einrichtung bleiben weiterhin wirksam. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [AsFlatOpc](../../aspose.cells/pptxsaveoptions/asflatopc/) { get; set; } | Gibt an, ob als flache OPC‑Datei gespeichert wird, die mit dem Open XML SDK erzeugt werden kann |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Der Ordner für temporäre Dateien, der als Daten-Cache verwendet werden kann.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Ob Einschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, wird er abgeschnitten.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | Gibt an, ob die Schriftartkompatibilität für jedes Zeichen im Text überprüft werden soll. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | Wenn Zeichen in Excel Unicode sind und im Zellenstil nicht mit der richtigen Schriftart festgelegt wurden, können sie im PDF/Bild als Block erscheinen. Setzen Sie dies auf true, um zunächst zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen darzustellen. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Leere das Arbeitsbuch nach dem Speichern der Datei.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | Liest oder legt benutzerdefinierte Einstellungen während des Renderns fest. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | Liest oder legt die Standardsprache für die Bearbeitung fest. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | Wenn Zeichen in Excel Unicode sind und im Zellenstil nicht mit der richtigen Schriftart festgelegt wurden, können sie im PDF/Bild als Block erscheinen. Setzen Sie die DefaultFont, z. B. MingLiu oder MS Gothic, um diese Zeichen darzustellen. Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode‑Zeichen anzuzeigen. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | Implementiert diese Schnittstelle, um DrawObject und Bound beim Rendern zu erhalten. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EmbedXlsxAsChartDataSource](../../aspose.cells/pptxsaveoptions/embedxlsxaschartdatasource/) { get; set; } | Gibt an, ob eine xlsx‑Datei als Datenquelle des Diagramms eingebettet wird. |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | Einstellung für das Rendern von EMF‑Metadateien. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ExportViewType](../../aspose.cells/pptxsaveoptions/exportviewtype/) { get; set; } | Liest und setzt den Anzeigetyp beim Exportieren nach PowerPoint. Der standardmäßige Exporttyp funktioniert wie beim Drucken. |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | Liest oder legt die Farbe der Gitternetzlinien fest. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | Liest oder legt den Typ der Gitternetzlinien fest. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | Gibt an, ob Sie den Fehler beim Rendern ausblenden möchten. Der Fehler kann ein Fehler bei Formen, Bildern, Diagrammen usw. sein. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [IgnoreHiddenRows](../../aspose.cells/pptxsaveoptions/ignorehiddenrows/) { get; set; } | Gibt an, ob versteckte Zeilen beim Konvertieren von Excel nach PowerPoint ignoriert werden. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | Gibt an, ob nur die Schriftart des Zeichens ersetzt werden soll, wenn die Zellen­schriftart nicht kompatibel ist. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße der Seiten­einrichtung wird ungültig sein, und die anderen Einstellungen der Seiten­einrichtung bleiben weiterhin wirksam. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | Liest oder legt die Anzahl der zu speichernden Seiten fest. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | Liest oder legt den nullbasierten Index der ersten zu speichernden Seite fest. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | Steuert/zeigt den Fortschritt des Seiten‑Speichervorgangs an. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | Gibt an, welche Seiten nicht gedruckt werden. (Vererbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | Liest oder legt das Excel-spezifische Rendering-Verhalten fest, das angewendet werden soll.(Geerbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SaveAsEditableShapes](../../aspose.cells/pptxsaveoptions/saveaseditableshapes/) { get; set; } | Speichere alle Zeichenobjekte als editierbare Formen in der PPTX‑Datei, sodass Sie sie in PowerPoint bearbeiten können. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Liest das Speicherdateiformat.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | Liest oder legt die zu rendernden Arbeitsblätter fest. Standard ist, dass alle sichtbaren Arbeitsblätter in der Arbeitsmappe verwendet werden: [`Visible`](../../aspose.cells.rendering/sheetset/visible/).(Geerbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | Liest oder legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist.(Geerbt von [`PaginatedSaveOptions`](../paginatedsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. Der Standardwert ist false.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Liest oder setzt den Warnungs-Callback.(Vererbt von [`SaveOptions`](../saveoptions/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using Aspose.Cells.Rendering;
    using System;

    public class PptxSaveOptionsDemo
    {
        public static void PptxSaveOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füllen Sie einige Daten in das Arbeitsblatt ein
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Erstelle eine Instanz von PptxSaveOptions
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                IgnoreHiddenRows = true,
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows,
                ExportViewType = SlideViewType.Print,
                DefaultFont = "Arial",
                CheckWorkbookDefaultFont = true,
                CheckFontCompatibility = true,
                IsFontSubstitutionCharGranularity = true,
                OnePagePerSheet = true,
                AllColumnsInOnePagePerSheet = true,
                IgnoreError = true,
                OutputBlankPageWhenNothingToPrint = true,
                PageIndex = 0,
                PageCount = 1,
                PrintingPageType = PrintingPageType.IgnoreBlank,
                GridlineType = GridlineType.Dotted,
                TextCrossType = TextCrossType.CrossKeep,
                DefaultEditLanguage = DefaultEditLanguage.English,
                SheetSet = SheetSet.Visible,
                EmfRenderSetting = EmfRenderSetting.EmfOnly,
                ClearData = true,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = true
            };

            // Speichere die Arbeitsmappe als PPTX‑Datei
            workbook.Save("PptxSaveOptionsExample.pptx", saveOptions);
        }
    }
}
```

### Siehe auch

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


