---
title: "Klass EbookLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.EbookLoadOptions-klass. Representerar alternativ när en e‑bokfil importeras"
type: docs
url: /sv/net/aspose.cells/ebookloadoptions/
---
## EbookLoadOptions class

Representerar alternativ när en e-bokfil importeras.

```csharp
public class EbookLoadOptions : HtmlLoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [EbookLoadOptions](ebookloadoptions/#constructor)() | Skapar ett alternativ för att läsa in e‑bokfilen. |
| [EbookLoadOptions](ebookloadoptions/#constructor_1)(LoadFormat) | Skapar ett alternativ för inläsning av e‑bokfilen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolete.**) Katalogen som de bifogade filerna kommer att sparas i.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Anger om data automatiskt filtreras vid inläsning av filerna.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | Anger om kolumner och rader ska auto‑anpassas. Standardvärdet är falskt.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Hämtar och anger auto‑fitter‑alternativen (Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Kontrollerar om data är giltiga i mallfilen.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32 K. När du anger ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Om du däremot har angett ett värde som är ogiltigt för Excel‑filformatet bör du inte spara arbetsboken som Excel‑format senare. Annars kan det uppstå oväntade fel i den genererade Excel‑filen.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till datumdata. Standardvärdet är true.(Ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolete.**) om sant, konvertera sträng till formel när strängvärdet börjar med tecknet '=',standardvärdet är falskt.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till numerisk data. Standardvärdet är true.(Ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för den arbetsbok som ska läsas in.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Hämtar standardstilinställningarna för att initiera stilar i arbetsboken (Inherited from [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | Anger om överflödiga mellanslag ska tas bort när texten radbryts med `<br>`-taggen. Standardvärdet är falskt.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | Anger om LaTeX‑formler ska upptäckas i HTML‑filen. Standardvärdet är falskt.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Hämtar och anger standardkodningen. Gäller endast för csv-filer. (ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för den [`Workbook`](../workbook/) som använder dessa [`LoadOptions`](../loadoptions/) för inläsning. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | Anger om texten är en formel om den börjar med "=".(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | Specificerar hur hyperlänkar laddas när HTML laddas.(Inherited from [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignorera data som inte skrivs ut om filen skrivs ut direkt (Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Anger om onödiga former ska ignoreras. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Hämtar och anger avbrottsmontorn. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Anger om en strängvärde inte ska parsas om längden är 15. (ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Om de oparserade data ska hållas i minnet för arbetsboken när den läses in från en mallfil. Standard är true. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Hämtar eller anger gränssnittsspråket för arbetsboksversionen baserat på CountryCode som sparade filen. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Datahanteraren för att bearbeta celldata när mallfilen läses. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Filtret som anger hur data ska läsas in. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Hämtar inläsningsformatet. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | Indikerar om formler importeras om den ursprungliga html-filen innehåller formler(ärvd från [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Anger strategin för att tillämpa stil på parsade värden när en strängvärde konverteras till nummer eller datum/tid. (ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Hämtar eller anger minnesläget för den inlästa arbetsboken. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolete.**) Anger hur HTML &lt;p&gt;-element renderas när HTML laddas. Standardvärdet är Normal.(ärvd från [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | Anger hur HTML &lt;p&gt;-element renderas när HTML laddas. Standardvärdet är Normal.(ärvd från [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Anger om formeln ska parsas när filen läses. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Anger om pivottabellens cachade poster ska parsas vid inläsning av filen. Standardvärdet är false. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Hämtar och anger lösenordet för arbetsboken. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Anger om mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | Hämtar program‑id för att skapa filen. Endast för MHT‑filer.(ärvd från [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för den arbetsbok som ska läsas in.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Föråldrad.**) Anger standardteckensnittets namn(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Föråldrad.**) Anger standardteckensnittets storlek.(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | Hämtar eller anger StreamProviderImportHtmlFile för att importera objekt.(ärvd från [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | Indikerar om layouten för `<div>`‑taggen stöds när html‑filen innehåller den. Standardvärdet är false.(ärvd från [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | Hämta HtmlTableLoadOptionCollection‑instansen(ärvd från [`HtmlLoadOptions`](../htmlloadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranropet.(Ärvd från [`LoadOptions`](../loadoptions/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Anger standardpappersstorlek för utskrift från standardskrivarens inställning.(Ärvd från [`LoadOptions`](../loadoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;
    using System.Text;

    public class EbookLoadOptionsDemo
    {
        public static void EbookLoadOptionsExample()
        {
            // Skapa en instans av EbookLoadOptions
            EbookLoadOptions options = new EbookLoadOptions();

            // Ställa in egenskaper
            options.AttachedFilesDirectory = "C:\\AttachedFiles";
            options.LoadFormulas = true;
            options.SupportDivTag = true;
            options.DeleteRedundantSpaces = true;
            options.AutoFitColsAndRows = true;
            options.ConvertFormulasData = true;
            options.HasFormula = true;
            options.Encoding = Encoding.UTF8;
            options.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            options.ConvertNumericData = true;
            options.ConvertDateTimeData = true;
            options.KeepPrecision = true;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = true;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            options.StandardFont = "Arial";
            options.StandardFontSize = 12.0;
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter();
            options.LightCellsDataHandler = null; // Assuming no light cells data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = new IndividualFontConfigs();
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = true;

            // Läs in en e‑bokfil i en arbetsbok med de angivna alternativen
            Workbook workbook = new Workbook("EbookLoadOptionsExample_original.ebook", options);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("EbookLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [HtmlLoadOptions](../htmlloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


