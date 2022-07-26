---
title: ImageOrPrintOptions
second_title: Aspose.Cells für .NET-API-Referenz
description: Ermöglicht das Festlegen von Optionen beim Rendern von Arbeitsblättern in Bilder Drucken von Arbeitsblättern oder Rendern von Diagrammen in Bilder.
type: docs
weight: 5140
url: /de/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Ermöglicht das Festlegen von Optionen beim Rendern von Arbeitsblättern in Bilder, Drucken von Arbeitsblättern oder Rendern von Diagrammen in Bilder.

```csharp
public class ImageOrPrintOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet) { get; set; } | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts als Ergebnis nur auf einer Seite ausgegeben. Die Breite des Papierformats von pagesetup wird ungültig, und die anderen Einstellungen von pagesetup werden weiterhin wirksam. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont) { get; set; } | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt werden, Sie können als Block im PDF-Bild erscheinen. Setzen Sie dies auf „true“, um zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen zuerst anzuzeigen. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler) { get; set; } | Der Client kann beim Drucken jeder Seite mit diesem EventHandler eine spezielle Ausgabe an den Drucker vornehmen |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler) { get; set; } | Der Client kann die Seiteneinstellung des Druckers steuern, wenn jede Seite mit diesem EventHandler gedruckt wird |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage) { get; set; } | Ruft die Standardbearbeitungssprache ab oder legt sie fest. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont) { get; set; } | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt werden, Sie können als Block in pdf,image erscheinen. Legen Sie die DefaultFont wie MingLiu oder MS Gothic fest, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft ist nicht festgelegt, verwendet Aspose.Cells die Standardschrift des Systems, um diese Unicode-Zeichen anzuzeigen. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler) { get; set; } | Implementiert diese Schnittstelle, um DrawObject und Bound beim Rendern zu erhalten. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg) { get; set; } | Geben Sie den Dateinamen des eingebetteten Bildes in SVG an. Dies sollte ein vollständiger Pfad mit einem Verzeichnis wie "c:\\xpsEmbedded" sein |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype) { get; set; } | Ruft einen EmfType ab oder legt ihn fest, der das Format der Metadatei angibt.. Der Standardwert ist EmfPlusDual. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype) { get; set; } | Ruft den Rasterlinientyp ab oder legt ihn fest. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution) { get; set; } | Ruft die horizontale Auflösung für generierte Bilder in Punkten pro Zoll ab oder legt sie fest. Wendet die Bildgenerierungsmethode mit Ausnahme von Bildern im EMF-Format an. |
| [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype) { get; set; } | Holt oder setzt das Format der generierten Bilder. Standardwert: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit) { get; set; } | Gibt an, ob die Breite und Höhe der Zellen automatisch an den Zellenwert angepasst wird. Der Standardwert ist falsch. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity) { get; set; } | Gibt an, ob die Zeichenschrift nur dann ersetzt werden soll, wenn die Zellenschrift nicht damit kompatibel ist. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized) { get; set; } | Gibt an, ob die Ausgabeelemente optimiert werden sollen. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet) { get; set; } | Wenn OnePagePerSheet wahr ist, wird der gesamte Inhalt eines Blatts als Ergebnis nur auf einer Seite ausgegeben. Das Papierformat von pagesetup wird ungültig, und die anderen Einstellungen von pagesetup werden weiterhin wirksam. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea) { get; set; } | Wenn diese Eigenschaft wahr ist, wird ein Bereich ausgegeben, und es wird keine Skalierung wirksam. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint) { get; set; } | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount) { get; set; } | Ruft die Anzahl der zu speichernden Seiten ab oder legt sie fest. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex) { get; set; } | Ruft den 0-basierten Index der ersten zu speichernden Seite ab oder legt ihn fest. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback) { get; set; } | Steuerung/Fortschritt des Seitenspeichervorgangs anzeigen. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat) { get; set; } | Ruft das Pixelformat für die generierten Bilder ab oder legt es fest. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage) { get; set; } | Gibt an, welche Seiten nicht gedruckt werden. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog) { get; set; } | Wenn PrintWithStatusDialog = true , wird ein Dialogfeld angezeigt, das den aktuellen Druckstatus anzeigt. andernfalls wird kein solches Dialogfeld angezeigt. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der die Qualität der generierten Bilder bestimmt , die nur angewendet werden, wenn Seiten in gespeichert werden`JPEG` Format. Der Standardwert ist 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat) { get; set; } | Ruft das Ausgabedateiformat ab oder legt es fest type Unterstützt Tiff/XPS |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode) { get; set; } | Gibt an, ob Glättung (Antialiasing) auf Linien und Kurven und die Kanten gefüllter Bereiche angewendet wird. Der Standardwert ist SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport) { get; set; } | Wenn diese Eigenschaft wahr ist, passt das generierte SVG zum Ansichtsport. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype) { get; set; } | Ruft die Anzeige des Texttyps ab oder legt sie fest, wenn die Textbreite größer als die Zellenbreite ist. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint) { get; set; } | Gibt die Qualität der Textwiedergabe an. Der Standardwert ist TextRenderingHint.SystemDefault |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth) { get; set; } | Ruft die Bittiefe ab oder legt sie fest, die nur angewendet wird, wenn Seiten in gespeichert werden`Tiff` Format. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression) { get; set; } | Ruft den Komprimierungstyp ab oder legt ihn fest, der nur angewendet wird, wenn Seiten in gespeichert werden`Tiff` format. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent) { get; set; } | Gibt an, ob der Hintergrund des generierten Bildes transparent sein soll. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution) { get; set; } | Ruft die vertikale Auflösung für generierte Bilder in Punkten pro Zoll ab oder legt sie fest. Wendet die Bildgenerierungsmethode mit Ausnahme von Bildern im EMF-Format an. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback) { get; set; } | Ruft Warnrückruf ab oder legt ihn fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize)(int, int) | Legt die gewünschte Breite und Höhe des Bildes fest. |

### Beispiele

```csharp

[C#]

// Bild- oder Druckoptionen festlegen
ImageOrPrintOptions options = new ImageOrPrintOptions();

// Ausgabebildformat festlegen
options.ImageType = ImageType.Png;

// Horizontale Auflösung einstellen
options.HorizontalResolution = 300;

// Vertikale Auflösung einstellen
options.VerticalResolution = 300;

// Arbeitsmappe instanziieren
Workbook book = new Workbook("test.xls");

//Diagramm mit ImageOrPrint-Optionen als Bild speichern
book.Worksheets[0].Charts[0].ToImage("chart.png", options);

[VB.NET]

'Legen Sie die Bild- oder Druckoptionen fest
Dim options As New ImageOrPrintOptions()

'Ausgabebildformat festlegen
options.ImageType = ImageType.Png

'Stellen Sie die horizontale Auflösung ein
options.HorizontalResolution = 300

'Stellen Sie die vertikale Auflösung ein
options.VerticalResolution = 300

'Arbeitsmappe instanziieren
Dim book As New Workbook("test.xls")

'Speichern Sie das Diagramm als Bild mit den ImageOrPrint-Optionen
book.Worksheets(0).Charts(0).ToImage("chart.png", options)
```

### Siehe auch

* namensraum [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
