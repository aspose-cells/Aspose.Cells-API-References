---
title: "Klass GridImageOrPrintOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridDesktop.Data.GridImageOrPrintOptions-klass. Tillåter att specificera alternativ när kalkylblad renderas till bilder, skrivs ut eller när diagram renderas till bild"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridimageorprintoptions/
---
## GridImageOrPrintOptions class

Tillåter att ange alternativ när ett arbetsblad renderas till bilder, skrivs ut eller när ett diagram renderas till bild.

```csharp
public class GridImageOrPrintOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [GridImageOrPrintOptions](gridimageorprintoptions/)() | Konstruktionen av GridImageOrPrintOptions |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Om AllColumnsInOnePagePerSheet är sant, kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på pappersstorleken i sidinställningarna blir ogiltig, men de övriga inställningarna för sidinställningarna förblir aktiva. |
| [CheckWorkbookDefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/checkworkbookdefaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta på true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken. |
| [DefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/defaultfont/) { get; set; } | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är angiven kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode‑tecken. |
| [EmbededImageNameInSvg](../../aspose.cells.griddesktop.data/gridimageorprintoptions/embededimagenameinsvg/) { get; set; } | Ange filnamnet för den inbäddade bilden i SVG. Detta bör vara en fullständig sökväg med katalog, t.ex. "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/emftype/) { get; set; } | Hämtar eller anger en EmfType som specificerar formatet för Metafilen. Standardvärdet är EmfPlusDual. |
| [GridlineType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/gridlinetype/) { get; set; } | Hämtar eller anger typ av rutnätslinje. |
| [HorizontalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/horizontalresolution/) { get; set; } | Hämtar eller anger den horisontella upplösningen för genererade bilder, i punkter per tum. Tillämpas på bildgenereringsmetoden förutom EMF-formatbilder. |
| [ImageType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/imagetype/) { get; set; } | Hämtar eller anger formatet för de genererade bilderna. standardvärde: PNG. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt. |
| [IsOptimized](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isoptimized/) { get; set; } | Anger om utdataelementen ska optimeras. |
| [OnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onepagepersheet/) { get; set; } | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup kommer fortfarande att gälla. |
| [OnlyArea](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onlyarea/) { get; set; } | Om denna egenskap är sann, kommer ett område att skrivas ut och ingen skalning kommer att tillämpas. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [PageCount](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pagecount/) { get; set; } | Hämtar eller anger antalet sidor som ska sparas. |
| [PageIndex](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pageindex/) { get; set; } | Hämtar eller anger det 0‑baserade indexet för den första sidan som ska sparas. |
| [PixelFormat](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pixelformat/) { get; set; } | Hämtar eller anger pixelformatet för de genererade bilderna. |
| [PrintingPage](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printingpage/) { get; set; } | Anger vilka sidor som inte kommer att skrivas ut. |
| [PrintWithStatusDialog](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printwithstatusdialog/) { get; set; } | Om PrintWithStatusDialog = true visas en dialog som visar aktuell utskriftsstatus. Annars visas ingen sådan dialog. |
| [Quality](../../aspose.cells.griddesktop.data/gridimageorprintoptions/quality/) { get; set; } | Hämtar eller anger ett värde som bestämmer kvaliteten på de genererade bilderna, som endast tillämpas när sidor sparas i `Jpeg`‑formatet. Standardvärdet är 100. |
| [SmoothingMode](../../aspose.cells.griddesktop.data/gridimageorprintoptions/smoothingmode/) { get; set; } | Anger om utjämning (kantutjämning) tillämpas på linjer och kurvor samt kanterna på fyllda områden. Standardvärdet är SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.griddesktop.data/gridimageorprintoptions/svgfittoviewport/) { get; set; } | Om denna egenskap är sann, kommer den genererade svg att anpassas till visningsporten. |
| [TextCrossType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textcrosstype/) { get; set; } | Hämtar eller anger visningstyp för text när textbredden är större än cellbredden. |
| [TextRenderingHint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textrenderinghint/) { get; set; } | Anger kvaliteten på textåtergivning. Standardvärdet är TextRenderingHint.SystemDefault |
| [Transparent](../../aspose.cells.griddesktop.data/gridimageorprintoptions/transparent/) { get; set; } | Anger om bakgrunden på den genererade bilden ska vara transparent. |
| [VerticalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/verticalresolution/) { get; set; } | Hämtar eller anger den vertikala upplösningen för genererade bilder, i punkter per tum. Tillämpas på bildgenereringsmetoden förutom EMF-formatbilder. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setdesiredsize/)(int, int) | Anger önskad bredd och höjd på bilden. |
| [setRenderSheetSet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setrendersheetset/)(int[]) | Anger vilka blad som ska renderas. Standard är alla synliga blad i arbetsboken. Nollbaserade bladindex. |

### Se även

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


