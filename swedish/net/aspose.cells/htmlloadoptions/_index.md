---
title: "Klass HtmlLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HtmlLoadOptions klass. Representerar alternativ när en HTML-fil importeras"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/
---
## HtmlLoadOptions class

Representerar alternativ när en HTML-fil importeras.

```csharp
public class HtmlLoadOptions : AbstractTextLoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [HtmlLoadOptions](htmlloadoptions/#constructor)() | Skapar alternativ för att läsa in filen. |
| [HtmlLoadOptions](htmlloadoptions/#constructor_1)(LoadFormat) | Skapar alternativ för att läsa in filen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolete.**) Katalogen som de bifogade filerna kommer att sparas i. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Anger om data automatiskt filtreras vid inläsning av filerna.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | Anger om kolumner och rader ska auto-anpassas. Standardvärdet är falskt. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Hämtar och anger auto‑fitter‑alternativen (Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Kontrollerar om data är giltiga i mallfilen.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32 K. När du anger ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Om du däremot har angett ett värde som är ogiltigt för Excel‑filformatet bör du inte spara arbetsboken som Excel‑format senare. Annars kan det uppstå oväntade fel i den genererade Excel‑filen.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till datumdata. Standardvärdet är true.(Ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolete.**) om true, konvertera strängen till en formel när strängvärdet börjar med tecknet '=', standardvärdet är false. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till numerisk data. Standardvärdet är true.(Ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för den arbetsbok som ska läsas in.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Hämtar standardstilinställningarna för att initiera stilar i arbetsboken (Inherited from [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | Anger om överflödiga mellanslag ska tas bort när texten radbryts med `<br>`-taggen. Standardvärdet är false. |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | Anger om LaTeX-formler ska upptäckas i HTML-filen. Standardvärdet är false. |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Hämtar och anger standardkodningen. Gäller endast för csv-filer. (ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för den [`Workbook`](../workbook/) som använder dessa [`LoadOptions`](../loadoptions/) för inläsning. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | Anger om texten är en formel om den börjar med "=". |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | Anger hur hyperlänkar laddas när HTML laddas. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignorera data som inte skrivs ut om filen skrivs ut direkt (Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Anger om onödiga former ska ignoreras. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Hämtar och anger avbrottsmontorn. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Anger om en strängvärde inte ska parsas om längden är 15. (ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Om de oparserade data ska hållas i minnet för arbetsboken när den läses in från en mallfil. Standard är true. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Hämtar eller anger gränssnittsspråket för arbetsboksversionen baserat på CountryCode som sparade filen. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Datahanteraren för att bearbeta celldata när mallfilen läses. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Filtret som anger hur data ska läsas in. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Hämtar inläsningsformatet. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | Anger om formler ska importeras om den ursprungliga html-filen innehåller formler |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Anger strategin för att tillämpa stil på parsade värden när en strängvärde konverteras till nummer eller datum/tid. (ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Hämtar eller anger minnesläget för den inlästa arbetsboken. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolete.**) Anger hur HTML &lt;p&gt;-element renderas när HTML laddas. Standardvärdet är Normal. |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | Anger hur HTML &lt;p&gt;-element renderas när HTML laddas. Standardvärdet är Normal. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Anger om formeln ska parsas när filen läses. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Anger om pivottabellens cachade poster ska parsas vid inläsning av filen. Standardvärdet är false. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Hämtar och anger lösenordet för arbetsboken. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Anger om mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | Hämtar program‑id för att skapa filen. Gäller endast för MHT-filer. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för den arbetsbok som ska läsas in.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Föråldrad.**) Anger standardteckensnittets namn(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Föråldrad.**) Anger standardteckensnittets storlek.(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | Hämtar eller anger StreamProviderImportHtmlFile för att importera objekt. |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | Anger om layouten för `<div>`-taggen stöds när html-filen innehåller den. Standardvärdet är false. |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | Hämta HtmlTableLoadOptionCollection‑instansen |
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

    public class HtmlLoadOptionsDemo
    {
        public static void HtmlLoadOptionsExample()
        {
            // Skapa en instans av HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            loadOptions.LoadFormulas = true;
            loadOptions.SupportDivTag = true;
            loadOptions.DeleteRedundantSpaces = true;
            loadOptions.AutoFitColsAndRows = true;
            loadOptions.HasFormula = true;
            loadOptions.Encoding = System.Text.Encoding.UTF8;
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            loadOptions.ConvertNumericData = true;
            loadOptions.ConvertDateTimeData = true;
            loadOptions.KeepPrecision = true;
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = true;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = true;
            loadOptions.KeepUnparsedData = true;
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = true;

            // Läs in en HTML-fil i en arbetsbok med HtmlLoadOptions
            Workbook workbook = new Workbook("HtmlLoadOptionsExample_original.html", loadOptions);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("HtmlLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


