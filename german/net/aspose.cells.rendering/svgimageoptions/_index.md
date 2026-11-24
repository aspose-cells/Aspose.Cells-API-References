---
title: "Klasse SvgImageOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.SvgImageOptions class. Optionen zur Erzeugung von SVG-Bildern"
type: docs
url: /de/net/aspose.cells.rendering/svgimageoptions/
---
## SvgImageOptions class

Optionen zum Erzeugen von SVG‑Bildern.

```csharp
public class SvgImageOptions : ImageOrPrintOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SvgImageOptions](svgimageoptions/)() | Ctor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße des Seitenlayouts wird ungültig, und die anderen Einstellungen des Seitenlayouts bleiben wirksam. (Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Gibt den Bildtyp des Diagramms beim Konvertieren an. Standardwert: PNG. (Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Wenn Zeichen in Excel Unicode sind und im Zellstil nicht mit der richtigen Schriftart festgelegt wurden, können sie in PDF/Bild als Block dargestellt werden. Setzen Sie diesen Wert auf true, um zunächst zu versuchen, die Standardschriftart der Arbeitsmappe für diese Zeichen zu verwenden. (Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CssPrefix](../../aspose.cells.rendering/svgimageoptions/cssprefix/) { get; set; } | Ermittelt und legt das Präfix des CSS-Namens in SVG fest, der Standardwert ist eine leere Zeichenkette. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Der Client kann eine spezielle Ausgabe zum Drucker vornehmen, wenn jede Seite mit diesem EventHandler gedruckt wird (Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Der Client kann die Seiteneinstellungen des Druckers steuern, wenn jede Seite mit diesem EventHandler gedruckt wird (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Liest oder setzt benutzerdefinierte Einstellungen während des Renderns (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Liest oder setzt die Standardsprache für die Bearbeitung (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie im PDF oder Bild als Block erscheinen. Setzen Sie die DefaultFont, z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht gesetzt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode‑Zeichen darzustellen (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmbeddedFontType](../../aspose.cells.rendering/svgimageoptions/embeddedfonttype/) { get; set; } | Liest oder setzt den Typ der Schriftart, die in SVG eingebettet ist. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Gibt den Dateinamen des eingebetteten Bildes in SVG an. Dies sollte ein voller Pfad mit Verzeichnis sein, z. B. "c:\\xpsEmbedded" (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Einstellung für das Rendern von EMF-Metadateien in der Quelldatei (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Liest oder setzt einen EmfType, der das Format der Metadatei angibt. Der Standardwert ist EmfPlusDual (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [FitToViewPort](../../aspose.cells.rendering/svgimageoptions/fittoviewport/) { get; set; } | Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG an den Viewport an. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Liest oder setzt die Rasterlinienfarbe (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Liest oder setzt den Rasterlinientyp (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Liest oder setzt die horizontale Auflösung für erzeugte Bilder in DPI (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| override [ImageType](../../aspose.cells.rendering/svgimageoptions/imagetype/) { get; set; } | Liest oder setzt das Format der erzeugten Bilder. Standardwert: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Gibt an, ob Breite und Höhe der Zellen automatisch an den Zellenwert angepasst werden. Der Standardwert ist false (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Gibt an, ob nur die Schriftart des Zeichens ersetzt wird, wenn die Zellen‑Schriftart nicht kompatibel ist (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Gibt an, ob die Ausgabeelemente optimiert werden sollen (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Wenn OnePagePerSheet wahr ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße der Seiten­einrichtung wird ungültig, während die anderen Einstellungen der Seiten­einrichtung weiterhin wirksam bleiben (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Wenn diese Eigenschaft wahr ist, wird ein Bereich ausgegeben, und keine Skalierung wird wirksam (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist (geerbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Liest oder setzt die Anzahl der zu speichernden Seiten.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Liest oder setzt den nullbasierten Index der ersten zu speichernden Seite.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Steuert/zeigt den Fortschritt des Seiten‑Speichervorgangs an.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Liest oder setzt das Pixelformat für die erzeugten Bilder.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Gibt an, welche Seiten nicht gedruckt werden.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Wenn PrintWithStatusDialog = true ist, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt. andernfalls wird kein solcher Dialog angezeigt.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Liest oder setzt einen Wert, der die Qualität der erzeugten Bilder bestimmt und nur beim Speichern von Seiten im `Jpeg`‑Format angewendet wird. Der Standardwert ist 100.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Liest oder setzt den Ausgabedateiformattyp. Unterstützt Tiff/XPS.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Liest oder setzt die zu rendernden Tabellenblätter. Standard ist, dass alle sichtbaren Tabellenblätter in der Arbeitsmappe gerendert werden: [`Visible`](../sheetset/visible/).(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Gibt an, ob Glättung (Antialiasing) auf Linien, Kurven und die Kanten gefüllter Bereiche angewendet wird. Der Standardwert ist SmoothingMode.None.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Liest und setzt das Präfix des CSS‑Namens in SVG, der Standardwert ist eine leere Zeichenkette.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) Wenn diese Eigenschaft true ist, passt das erzeugte SVG an den Viewport an.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Liest oder setzt den Anzeigetexttyp, wenn die Textbreite größer als die Zellenbreite ist.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Gibt die Qualität der Textdarstellung an. Der Standardwert ist TextRenderingHint.SystemDefault.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Liest oder setzt die Methode, die beim Konvertieren von Bildern in das 1‑bpp‑Format verwendet wird, wenn [`ImageType`](../imageorprintoptions/imagetype/) Tiff ist und [`TiffCompression`](../imageorprintoptions/tiffcompression/) gleich Ccitt3 oder Ccitt4 ist.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Liest oder setzt die Bit‑Tiefe, die nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Liest oder setzt den Kompressionstyp, der nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Liest oder setzt die vertikale Auflösung für erzeugte Bilder in Punkten pro Zoll.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Liest oder setzt den Warnungs-Callback.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int) | (**Veraltet.**) Setzt die gewünschte Breite und Höhe des Bildes.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int, bool) | Setzt die gewünschte Breite und Höhe des Bildes.(Vererbt von [`ImageOrPrintOptions`](../imageorprintoptions/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgImageOptionsDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fülle Beispieldaten für das Diagramm
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(12000);
            worksheet.Cells["A3"].PutValue(16500);
            worksheet.Cells["B1"].PutValue("Q2");
            worksheet.Cells["B2"].PutValue(25500);
            worksheet.Cells["B3"].PutValue(10800);

            // Erstelle ein Säulendiagramm
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Initialisiere SVG-Bildoptionen
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Konfiguriere SVG-Renderoptionen
            svgOptions.FitToViewPort = true;
            svgOptions.CssPrefix = "chart-";
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
            svgOptions.ImageType = ImageType.Svg;

            // Setze Druckqualität und Auflösung
            svgOptions.PrintWithStatusDialog = true;
            svgOptions.HorizontalResolution = 300;
            svgOptions.VerticalResolution = 300;

            // Render das Diagramm nach SVG mit konfigurierten Optionen
            chart.ToImage("chart_output.svg", svgOptions);

            // Demonstriere die Integration des Arbeitsmappen-Speicherns
            workbook.Save("SvgRenderingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../imageorprintoptions/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


