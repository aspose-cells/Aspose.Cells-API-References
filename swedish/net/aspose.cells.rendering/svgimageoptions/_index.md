---
title: "Klass SvgImageOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.SvgImageOptions-klass. Alternativ för att generera Svg-bild"
type: docs
url: /sv/net/aspose.cells.rendering/svgimageoptions/
---
## SvgImageOptions class

Alternativ för att generera SVG‑bild.

```csharp
public class SvgImageOptions : ImageOrPrintOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SvgImageOptions](svgimageoptions/)() | Konstruktor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Om AllColumnsInOnePagePerSheet är sant, kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på papperstorleken i sidinställning blir ogiltig, och de andra inställningarna för sidinställning kommer fortfarande att tillämpas. (Ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Ange diagrammets bildtyp vid konvertering. standardvärde: PNG. (Ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta på true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken. (Ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CssPrefix](../../aspose.cells.rendering/svgimageoptions/cssprefix/) { get; set; } | Hämtar och anger prefixet för css-namnet i svg, standardvärdet är en tom sträng. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Klienten kan speciellt skriva ut till skrivare när varje sida skrivs ut med denna EventHandler (Ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Klienten kan kontrollera sidinställningarna för skrivaren när varje sida skrivs ut med denna EventHandler(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Hämtar eller anger anpassade inställningar under rendering.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Hämtar eller anger standardspråket för redigering.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen, kan de visas som block i pdf, bild. Ange DefaultFont såsom MingLiu eller MS Gothic för att visa dessa tecken. Om denna egenskap inte är inställd, kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmbeddedFontType](../../aspose.cells.rendering/svgimageoptions/embeddedfonttype/) { get; set; } | Hämtar eller anger typen av teckensnitt som är inbäddat i Svg. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Indikerar filnamnet på den inbäddade bilden i svg. Detta bör vara en fullständig sökväg med katalog som "c:\\xpsEmbedded"(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Inställning för rendering av Emf-metafiler i källfilen.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Hämtar eller anger en EmfType som specificerar formatet för Metafilen.. Standardvärdet är EmfPlusDual.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [FitToViewPort](../../aspose.cells.rendering/svgimageoptions/fittoviewport/) { get; set; } | Om denna egenskap är sann, kommer den genererade svg att anpassas till visningsporten. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Hämtar eller anger färg på rutnätslinjer.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Hämtar eller anger typ av rutnätslinje.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Hämtar eller anger den horisontella upplösningen för genererade bilder, i punkter per tum.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| override [ImageType](../../aspose.cells.rendering/svgimageoptions/imagetype/) { get; set; } | Hämtar eller anger formatet för de genererade bilderna. standardvärde: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Anger om bredden och höjden på cellerna automatiskt anpassas efter cellvärdet. Standardvärdet är false.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt med det.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Anger om utdataelementen ska optimeras.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Om OnePagePerSheet är true, kommer allt innehåll i ett blad att skrivas ut till endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de andra inställningarna i pagesetup kommer fortfarande att gälla.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Om denna egenskap är true, kommer ett område att skrivas ut, och ingen skalning kommer att tillämpas.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Hämtar eller anger antalet sidor att spara.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Hämtar eller anger det 0-baserade indexet för den första sidan att spara.(ärvd från [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Styr/indikera framsteg för sidlagringsprocessen.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Hämtar eller anger pixelformatet för de genererade bilderna.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Anger vilka sidor som inte kommer att skrivas ut.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Om PrintWithStatusDialog = true, kommer en dialog att visas som visar aktuell utskriftsstatus. annars visas ingen sådan dialog.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Hämtar eller anger ett värde som bestämmer kvaliteten på de genererade bilderna och som endast tillämpas när sidor sparas i `Jpeg`-formatet. Standardvärdet är 100(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Hämtar eller anger filformatstypen för utdata. Stöd för Tiff/XPS(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: [`Visible`](../sheetset/visible/).(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Anger om jämning (antialiasing) ska tillämpas på linjer och kurvor samt kanterna på fyllda områden. Standardvärdet är SmoothingMode.None(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Hämtar och anger prefixet för css-namnet i svg, standardvärdet är en tom sträng.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) om detta egenskap är true, kommer den genererade svg:n att anpassas till visningsporten.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Hämtar eller anger visningstyp för text när textbredden är större än cellbredden.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Anger kvaliteten på textåtergivning. Standardvärdet är TextRenderingHint.SystemDefault(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Hämtar eller anger metoden som används vid konvertering av bilder till 1 bpp-format när [`ImageType`](../imageorprintoptions/imagetype/) är Tiff och [`TiffCompression`](../imageorprintoptions/tiffcompression/) är lika med Ccitt3 eller Ccitt4.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Hämtar eller anger bitdjup som endast tillämpas när sidor sparas i `Tiff`-formatet.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Hämtar eller anger komprimeringstypen som endast tillämpas när sidor sparas i `Tiff`-formatet.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Anger om bakgrunden på den genererade bilden ska vara transparent.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Hämtar eller anger den vertikala upplösningen för genererade bilder, i punkter per tum.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int) | (**Obsolete.**) Anger önskad bredd och höjd för bilden.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int, bool) | Anger önskad bredd och höjd för bilden.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

### Exempel

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
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(12000);
            worksheet.Cells["A3"].PutValue(16500);
            worksheet.Cells["B1"].PutValue("Q2");
            worksheet.Cells["B2"].PutValue(25500);
            worksheet.Cells["B3"].PutValue(10800);

            // Skapa ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Initiera SVG‑alternativ för bild
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Konfigurera SVG‑renderingsalternativ
            svgOptions.FitToViewPort = true;
            svgOptions.CssPrefix = "chart-";
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
            svgOptions.ImageType = ImageType.Svg;

            // Ställ in utskriftskvalitet och upplösning
            svgOptions.PrintWithStatusDialog = true;
            svgOptions.HorizontalResolution = 300;
            svgOptions.VerticalResolution = 300;

            // Rendera diagram till SVG med konfigurerade alternativ
            chart.ToImage("chart_output.svg", svgOptions);

            // Demonstrera integration av arbetsbokssparning
            workbook.Save("SvgRenderingDemo.xlsx");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../imageorprintoptions/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


