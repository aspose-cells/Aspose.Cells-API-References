---
title: PdfSaveOptions
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert die Optionen zum Speichern der PDF-Datei.
type: docs
weight: 4500
url: /de/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Repräsentiert die Optionen zum Speichern der PDF-Datei.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions#constructor)() | Erstellt die Optionen zum Speichern der PDF-Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/pdfsaveoptions/allcolumnsinonepagepersheet) { get; set; } | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts als Ergebnis nur auf einer Seite ausgegeben. Die Breite des Papierformats von pagesetup wird ignoriert, und die anderen Einstellungen von pagesetup werden weiterhin wirksam. |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark) { get; set; } | Holt und setzt die[`PdfLesezeichenEintrag`](../../aspose.cells.rendering/pdfbookmarkentry) Objekt. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Der zwischengespeicherte Dateiordner wird verwendet, um einige große Daten zu speichern. |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula) { get; set; } | Gibt an, ob Formeln vor dem Speichern der PDF-Datei berechnet werden sollen. |
| [CheckFontCompatibility](../../aspose.cells/pdfsaveoptions/checkfontcompatibility) { get; set; } | Gibt an, ob die Schriftkompatibilität für jedes Zeichen im Text überprüft werden soll. |
| [CheckWorkbookDefaultFont](../../aspose.cells/pdfsaveoptions/checkworkbookdefaultfont) { get; set; } | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt werden, Sie können als Block im PDF-Bild erscheinen. Setzen Sie dies auf „true“, um zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen zuerst anzuzeigen. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Machen Sie die Arbeitsmappe nach dem Speichern der Datei leer. |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance) { get; set; } | Arbeitsmappe konvertiert in PDF wird gemäß PdfCompliance in dieser Eigenschaft. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis automatisch erstellt, bevor die Datei gespeichert wird. |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime) { get; set; } | Ermittelt und setzt die Uhrzeit der Generierung des PDF-Dokuments. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport) { get; set; } | Ruft oder setzt einen Wert, der den Weg bestimmt[`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection) werden in eine PDF-Datei exportiert. Der Standardwert ist None. |
| [DefaultEditLanguage](../../aspose.cells/pdfsaveoptions/defaulteditlanguage) { get; set; } | Ruft die Standardbearbeitungssprache ab oder legt sie fest. |
| [DefaultFont](../../aspose.cells/pdfsaveoptions/defaultfont) { get; set; } | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt werden, Sie können als Block in pdf,image erscheinen. Legen Sie die DefaultFont wie MingLiu oder MS Gothic fest, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft ist nicht festgelegt, verwendet Aspose.Cells die Standardschrift des Systems, um diese Unicode-Zeichen anzuzeigen. |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle) { get; set; } | Gibt an, ob die Titelleiste des Fensters den Dokumenttitel anzeigen soll. |
| [DrawObjectEventHandler](../../aspose.cells/pdfsaveoptions/drawobjecteventhandler) { get; set; } | Implementiert diese Schnittstelle, um DrawObject und Bound beim Rendern zu erhalten. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts) { get; set; } | True zum Einbetten von TrueType-Schriftarten. Betrifft nur die ASCII-Zeichen 32-127. Schriftarten für Zeichencodes größer als 127 werden immer eingebettet. Schriftarten werden immer für den Standard PDF/A-1a, PDF/A-1b eingebettet. Standard ist wahr. |
| [EmfRenderSetting](../../aspose.cells/pdfsaveoptions/emfrendersetting) { get; set; } | Einstellung zum Rendern der EMF-Metadatei. |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure) { get; set; } | Gibt an, ob die Dokumentstruktur exportiert werden soll. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding) { get; set; } | Ruft eingebettete Schriftcodierung in pdf ab oder legt sie fest. |
| [GridlineType](../../aspose.cells/pdfsaveoptions/gridlinetype) { get; set; } | Ruft den Rasterlinientyp ab oder legt ihn fest. |
| [IgnoreError](../../aspose.cells/pdfsaveoptions/ignoreerror) { get; set; } | Gibt an, ob Sie den Fehler beim Rendern ausblenden müssen. Der Fehler kann ein Fehler in der Form, im Bild, beim Rendern des Diagramms usw. sein. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/pdfsaveoptions/isfontsubstitutionchargranularity) { get; set; } | Gibt an, ob die Zeichenschrift nur dann ersetzt werden soll, wenn die Zellenschrift nicht damit kompatibel ist. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung zusammengeführt werden, bevor die Datei gespeichert wird. |
| [OnePagePerSheet](../../aspose.cells/pdfsaveoptions/onepagepersheet) { get; set; } | Wenn OnePagePerSheet wahr ist, wird der gesamte Inhalt eines Blatts als Ergebnis nur auf einer Seite ausgegeben. Das Papierformat von pagesetup wird ungültig, und die anderen Einstellungen von pagesetup werden weiterhin wirksam. |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype) { get; set; } | Ruft den PDF-Optimierungstyp ab und legt ihn fest. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/pdfsaveoptions/outputblankpagewhennothingtoprint) { get; set; } | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [PageCount](../../aspose.cells/pdfsaveoptions/pagecount) { get; set; } | Ruft die Anzahl der zu speichernden Seiten ab oder legt sie fest. |
| [PageIndex](../../aspose.cells/pdfsaveoptions/pageindex) { get; set; } | Ruft den 0-basierten Index der ersten zu speichernden Seite ab oder legt ihn fest. |
| [PageSavingCallback](../../aspose.cells/pdfsaveoptions/pagesavingcallback) { get; set; } | Steuerung/Fortschritt des Seitenspeichervorgangs anzeigen. |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression) { get; set; } | Geben Sie den Komprimierungsalgorithmus an |
| [PrintingPageType](../../aspose.cells/pdfsaveoptions/printingpagetype) { get; set; } | Gibt an, welche Seiten nicht gedruckt werden. |
| [Producer](../../aspose.cells/pdfsaveoptions/producer) { get; set; } | Ruft den Erzeuger des generierten PDF-Dokuments ab und legt ihn fest. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Gibt an, ob Diagramm-Cache-Daten aktualisiert werden |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Ruft das Sicherungsdateiformat ab. |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions) { get; set; } | Stellen Sie diese Optionen ein, wenn Sicherheit im xls2pdf-Ergebnis benötigt wird. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Gibt an, ob extern definierte Namen vor dem Speichern der Datei sortiert werden. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [TextCrossType](../../aspose.cells/pdfsaveoptions/textcrosstype) { get; set; } | Ruft die Anzeige des Texttyps ab oder legt sie fest, wenn die Textbreite größer als die Zellenbreite ist. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Gibt an, ob die SmartArt-Einstellung aktualisiert wird. Der Standardwert ist „false“. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Gibt an, ob verbundene Zellen validiert werden sollen, bevor die Datei gespeichert wird. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Ruft Warnrückruf ab oder legt ihn fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample)(int, int) | Legt die gewünschte PPI (Pixel pro Zoll) von Resample-Bildern und JPEG-Qualität fest. Alle Bilder werden mit der angegebenen Qualitätseinstellung in JPEG konvertiert, und Bilder, die größer als die angegebene PPI (Pixel pro Zoll) sind, werden neu berechnet. |

### Siehe auch

* class [SaveOptions](../saveoptions)
* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
