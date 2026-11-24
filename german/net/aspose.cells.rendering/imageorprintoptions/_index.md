---
title: "Klasse ImageOrPrintOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.ImageOrPrintOptions‑Klasse. Ermöglicht das Festlegen von Optionen beim Rendern von Arbeitsblättern zu Bildern, beim Drucken von Arbeitsblättern oder beim Rendern von Diagrammen zu Bildern."
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Ermöglicht das Festlegen von Optionen beim Rendern von Arbeitsblättern zu Bildern, beim Drucken von Arbeitsblättern oder beim Rendern von Diagrammen zu Bildern.

```csharp
public class ImageOrPrintOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions/)() | Ctor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße der pagesetup wird ungültig sein, und die anderen Einstellungen der pagesetup bleiben wirksam. |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Gibt den Bildtyp des Diagramms beim Konvertieren an. Standardwert: PNG. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Wenn Zeichen in der Excel-Datei Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie als Block in PDF oder Bild erscheinen. Setzen Sie diesen Wert auf true, um zunächst zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen anzuzeigen. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Der Client kann eine spezielle Ausgabe zum Drucker vornehmen, wenn jede Seite mit diesem EventHandler gedruckt wird. |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Der Client kann die Seiteneinstellungen des Druckers steuern, wenn jede Seite mit diesem EventHandler gedruckt wird. |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Liest oder legt benutzerdefinierte Einstellungen während des Renderns fest. |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Liest oder setzt die Standardsprache für die Bearbeitung. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Wenn Zeichen in der Excel-Datei Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie als Block in PDF oder Bild erscheinen. Setzen Sie die DefaultFont, z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode‑Zeichen darzustellen. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implementiert dieses Interface, um beim Rendern DrawObject und Bound zu erhalten. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Gibt den Dateinamen des eingebetteten Bildes in SVG an. Dies sollte ein voller Pfad mit Verzeichnis sein, z. B. "c:\\xpsEmbedded" |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Einstellung zum Rendern von EMF-Metadateien in der Quelldatei. |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Ruft einen EmfType ab oder legt ihn fest, der das Format der Metafile angibt. Der Standardwert ist EmfPlusDual. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Ruft die gridline colr ab oder legt sie fest. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Liest oder legt den Typ der Gitternetzlinien fest. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Ruft die horizontale Auflösung für erzeugte Bilder ab oder legt sie fest, in Punkten pro Zoll. |
| virtual [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype/) { get; set; } | Liest oder setzt das Format der erzeugten Bilder. Standardwert: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Gibt an, ob Breite und Höhe der Zellen automatisch an den Zellenwert angepasst werden. Der Standardwert ist false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Gibt an, ob die Schriftart eines Zeichens nur dann ersetzt werden soll, wenn die Zellen‑Schriftart nicht kompatibel ist. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Gibt an, ob die Ausgabeelemente optimiert werden sollen. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Ist OnePagePerSheet true, wird der gesamte Inhalt eines Blatts im Ergebnis nur auf einer Seite ausgegeben. Die Papiergröße der Seiten­einstellungen wird ungültig, während die anderen Einstellungen der Seiten­einstellungen weiterhin wirksam bleiben. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Wenn diese Eigenschaft true ist, wird ein Area ausgegeben und keine Skalierung wirkt. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Liest oder legt die Anzahl der zu speichernden Seiten fest. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Liest oder legt den nullbasierten Index der ersten zu speichernden Seite fest. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Steuern/Anzeigen des Fortschritts des Seiten‑Speichervorgangs. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Ruft das Pixelformat für die erzeugten Bilder ab oder legt es fest. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Gibt an, welche Seiten nicht gedruckt werden. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Wenn PrintWithStatusDialog = true ist, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt. Andernfalls wird kein solcher Dialog angezeigt. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Ruft den Wert ab oder legt ihn fest, der die Qualität der erzeugten Bilder bestimmt und nur beim Speichern von Seiten im `Jpeg`‑Format angewendet wird. Der Standardwert ist 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Ruft den Ausgabedateiformattyp ab oder legt ihn fest. Unterstützt Tiff/XPS |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Ruft die zu rendernden Arbeitsblätter ab oder legt sie fest. Standard ist alle sichtbaren Arbeitsblätter in der Arbeitsmappe: [`Visible`](../sheetset/visible/). |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Gibt an, ob Glättung (Antialiasing) auf Linien, Kurven und die Kanten gefüllter Bereiche angewendet wird. Der Standardwert ist SmoothingMode.None |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Ruft das Präfix des CSS‑Namens in SVG ab und legt es fest, der Standardwert ist eine leere Zeichenkette. |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) Wenn diese Eigenschaft true ist, passt das erzeugte SVG an den Ansichtsbereich an. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Liest oder legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Gibt die Qualität der Textdarstellung an. Der Standardwert ist TextRenderingHint.SystemDefault |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Ruft die beim Konvertieren von Bildern in das 1‑bpp‑Format verwendete Methode ab oder legt sie fest, wenn [`ImageType`](./imagetype/) Tiff ist und [`TiffCompression`](./tiffcompression/) gleich Ccitt3 oder Ccitt4 ist. |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Ruft die Bittiefe ab oder legt sie fest, die nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Ruft den Kompressionstyp ab oder legt ihn fest, der nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Ruft die vertikale Auflösung für erzeugte Bilder ab oder legt sie fest, in Punkten pro Zoll. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Liest oder setzt den Warnungs-Callback. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize)(int, int) | (**Obsolete.**) Legt die gewünschte Breite und Höhe des Bildes fest. |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize_1)(int, int, bool) | Legt die gewünschte Breite und Höhe des Bildes fest. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class RenderingClassImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ImageOrPrintOptions und setze Eigenschaften
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Erstelle eine neue Arbeitsmappe mit Beispieldaten und Diagramm
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Speichere das Diagramm als Bild unter Verwendung der Optionen
            chart.ToImage("output_chart.png", options);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


