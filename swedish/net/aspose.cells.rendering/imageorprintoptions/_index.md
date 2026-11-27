---
title: "Klassen ImageOrPrintOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.ImageOrPrintOptions‑klassen. Gör det möjligt att ange alternativ när kalkylblad renderas till bilder, skrivs ut eller när diagram renderas till bild"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Tillåter att ange alternativ när ett arbetsblad renderas till bilder, skrivs ut eller när ett diagram renderas till bild.

```csharp
public class ImageOrPrintOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions/)() | Konstruktor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Om AllColumnsInOnePagePerSheet är sant, kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på pappersstorleken i sidinställningarna blir ogiltig, men de övriga inställningarna för sidinställningarna förblir aktiva. |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Ange diagrammets bildtyp vid konvertering. standardvärde: PNG. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta på true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Klienten kan särskilt skicka utskrift till skrivaren när varje sida skrivs ut med denna EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Klienten kan kontrollera sidinställningarna för skrivaren när varje sida skrivs ut med denna EventHandler |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Hämtar eller anger anpassade inställningar under rendering. |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Hämtar eller anger standardspråket för redigering. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är angiven kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode‑tecken. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implementerar detta gränssnitt för att hämta DrawObject och Bound vid rendering. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Ange filnamnet för den inbäddade bilden i svg. Detta bör vara en fullständig sökväg med katalog, t.ex. "c:\\xpsEmbedded" |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Inställning för rendering av Emf‑metafiler i källfilen. |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Hämtar eller anger en EmfType som specificerar formatet för Metafilen. Standardvärdet är EmfPlusDual. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Hämtar eller anger färg på rutnätslinjer. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Hämtar eller anger typ av rutnätslinje. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Hämtar eller anger den horisontella upplösningen för genererade bilder, i punkter per tum. |
| virtual [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype/) { get; set; } | Hämtar eller anger formatet för de genererade bilderna. standardvärde: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Anger om bredden och höjden på cellerna automatiskt anpassas efter cellvärdet. Standardvärdet är falskt. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Anger om utdataelementen ska optimeras. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup kommer fortfarande att gälla. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Om denna egenskap är sann, kommer ett område att skrivas ut och ingen skalning kommer att tillämpas. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Hämtar eller anger antalet sidor som ska sparas. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Hämtar eller anger det 0‑baserade indexet för den första sidan som ska sparas. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Styr/indikera framsteg för sidlagringsprocessen. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Hämtar eller anger pixelformatet för de genererade bilderna. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Anger vilka sidor som inte kommer att skrivas ut. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Om PrintWithStatusDialog = true visas en dialog som visar aktuell utskriftsstatus. Annars visas ingen sådan dialog. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Hämtar eller anger ett värde som bestämmer kvaliteten på de genererade bilderna, som endast tillämpas när sidor sparas i `Jpeg`‑formatet. Standardvärdet är 100. |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Hämtar eller anger filformatstypen för utdata. Stöder Tiff/XPS |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: [`Visible`](../sheetset/visible/). |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Anger om utjämning (kantutjämning) tillämpas på linjer och kurvor samt kanterna på fyllda områden. Standardvärdet är SmoothingMode.None |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Hämtar och anger prefixet för css‑namnet i svg, standardvärdet är en tom sträng |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) om den här egenskapen är sann, kommer den genererade svg:n att anpassas till visningsporten. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Hämtar eller anger visningstyp för text när textbredden är större än cellbredden. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Anger kvaliteten på textåtergivning. Standardvärdet är TextRenderingHint.SystemDefault |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Hämtar eller anger metod som används vid konvertering av bilder till 1 bpp-format när [`ImageType`](./imagetype/) är Tiff och [`TiffCompression`](./tiffcompression/) är lika med Ccitt3 eller Ccitt4. |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Hämtar eller anger bithöjd att tillämpa endast när sidor sparas i `Tiff`-formatet. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Hämtar eller anger komprimeringstyp att tillämpa endast när sidor sparas i `Tiff`-formatet. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Anger om bakgrunden på den genererade bilden ska vara transparent. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Hämtar eller anger vertikal upplösning för genererade bilder, i punkter per tum. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize)(int, int) | (**Obsolete.**) Anger önskad bredd och höjd på bilden. |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize_1)(int, int, bool) | Anger önskad bredd och höjd på bilden. |

### Exempel

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
            // Skapa ImageOrPrintOptions och ange egenskaper
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Skapa en ny arbetsbok med exempeldata och diagram
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Spara diagram som bild med hjälp av alternativen
            chart.ToImage("output_chart.png", options);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


