---
title: ImageOrPrintOptions
second_title: Aspose.Cells för .NET API-referens
description: Gör det möjligt att ange alternativ när du renderar kalkylblad till bilder skriver ut kalkylblad eller renderar diagram till bild.
type: docs
weight: 5140
url: /sv/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Gör det möjligt att ange alternativ när du renderar kalkylblad till bilder, skriver ut kalkylblad eller renderar diagram till bild.

```csharp
public class ImageOrPrintOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet) { get; set; } | Om AllColumnsInOnePagePerSheet är sant , kommer allt kolumninnehåll på ett ark att matas ut till endast en sida i resultat. Bredden på pappersstorleken för siduppsättningen kommer att vara ogiltig, och de andra inställningarna för siduppsättningen kommer fortfarande att gälla. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont) { get; set; } | När tecken i Excel är Unicode och inte är inställda med korrekt typsnitt i cellstil, kan de visas som block i pdf,image. Ställ in detta på sant för att försöka använda arbetsbokens standardteckensnitt för att visa dessa tecken först. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler) { get; set; } | Klient kan specialutmata skrivaren när varje sida skrivs ut med denna EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler) { get; set; } | Klienten kan styra sidinställningarna för skrivaren när varje sida skrivs ut med denna EventHandler |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage) { get; set; } | Hämtar eller ställer in standardspråk för redigering. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont) { get; set; } | När tecken i Excel är Unicode och inte är inställda med korrekt typsnitt i cellstil, kan de visas som block i pdf,image. Ställ in standardteckensnittet som MingLiu eller MS Gothic för att visa dessa tecken. Om denna egenskap är inte inställt, kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa unicode-tecken. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler) { get; set; } | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg) { get; set; } | Ange filnamnet på den inbäddade bilden i svg. Detta bör vara fullständig sökväg med katalog som "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype) { get; set; } | Hämtar eller ställer in en EmfType som anger formatet för metafilen.. Standardvärdet är EmfPlusDual. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype) { get; set; } | Hämtar eller ställer in rutnätstyp. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution) { get; set; } | Hämtar eller ställer in den horisontella upplösningen för genererade bilder, i punkter per tum. Använder genererande bildmetoden förutom bilder i EMF-format. |
| [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype) { get; set; } | Hämtar eller ställer in formatet för de genererade bilderna. standardvärde: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit) { get; set; } | Indikerar om bredden och höjden på cellerna automatiskt anpassas efter cellvärde. Standardvärdet är false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity) { get; set; } | Indikerar om teckensnittet endast ska bytas ut när cellteckensnittet inte är kompatibelt med det. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized) { get; set; } | Indikerar om utgångselementen ska optimeras. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet) { get; set; } | Om OnePagePerSheet är sant , kommer allt innehåll på ett ark att matas ut till endast en sida som resultat. Pappersstorleken för siduppsättningen kommer att vara ogiltig, och de andra inställningarna för siduppsättningen kommer fortfarande att gälla. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea) { get; set; } | Om den här egenskapen är true kommer ett område att matas ut, och ingen skala kommer att träda i kraft. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint) { get; set; } | Indikerar om en tom sida ska matas ut när det inte finns något att skriva ut. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount) { get; set; } | Hämtar eller ställer in antalet sidor som ska sparas. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex) { get; set; } | Hämtar eller ställer in det 0-baserade indexet för den första sidan som ska sparas. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback) { get; set; } | Kontrollera/indikera framsteg för sidsparprocessen. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat) { get; set; } | Hämtar eller ställer in pixelformatet för de genererade bilderna. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage) { get; set; } | Indikerar vilka sidor som inte kommer att skrivas ut. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog) { get; set; } | Om PrintWithStatusDialog = true kommer det att finnas en dialogruta som visar aktuell utskriftsstatus. annars visas ingen sådan dialog. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality) { get; set; } | Hämtar eller ställer in ett värde som bestämmer kvaliteten på de genererade bilderna för att endast gälla när sidor sparas till`Jpeg` formatera. Standardvärdet är 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat) { get; set; } | Hämtar eller ställer in utdatafilformatet type Support Tiff/XPS |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode) { get; set; } | Anger om utjämning (kantutjämning) tillämpas på linjer och kurvor och kanterna på fyllda områden. Standardvärdet är SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport) { get; set; } | om den här egenskapen är sann kommer den genererade svg att passa för att visa port. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype) { get; set; } | Hämtar eller ställer in visning av texttyp när textbredden är större än cellbredden. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint) { get; set; } | Anger kvaliteten på textrenderingen. Standardvärdet är TextRenderingHint.SystemDefault |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth) { get; set; } | Hämtar eller ställer in bitdjup för att endast tillämpas när sidor sparas till`Tiff` formatera. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression) { get; set; } | Hämtar eller ställer in typen av komprimering så att den endast tillämpas när sidor sparas i`Tiff` format. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent) { get; set; } | Indikerar om bakgrunden för den genererade bilden ska vara transparent. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution) { get; set; } | Hämtar eller ställer in den vertikala upplösningen för genererade bilder, i punkter per tum. Tillämpar genererande bildmetoden förutom Emf-formatbild. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback) { get; set; } | Får eller ställer in varningsåteruppringning. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize)(int, int) | Ställer in önskad bredd och höjd på bilden. |

### Exempel

```csharp

[C#]

//Ange bild- eller utskriftsalternativ
ImageOrPrintOptions options = new ImageOrPrintOptions();

//Ställ in bildformat för utdata
options.ImageType = ImageType.Png;

//Ställ in horisontell upplösning
options.HorizontalResolution = 300;

//Ställ in vertikal upplösning
options.VerticalResolution = 300;

//Instantiate Workbook
Workbook book = new Workbook("test.xls");

//Spara diagram som bild med ImageOrPrint-alternativ
book.Worksheets[0].Charts[0].ToImage("chart.png", options);

[VB.NET]

'Ställ in bild- eller utskriftsalternativ
Dim options As New ImageOrPrintOptions()

'Ställ in bildformat för utdata
options.ImageType = ImageType.Png

'Ställ in horisontell upplösning
options.HorizontalResolution = 300

'Ställ in vertikal upplösning
options.VerticalResolution = 300

'Instantiera arbetsbok
Dim book As New Workbook("test.xls")

'Spara diagram som bild med ImageOrPrint-alternativ
book.Worksheets(0).Charts(0).ToImage("chart.png", options)
```

### Se även

* namnutrymme [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
