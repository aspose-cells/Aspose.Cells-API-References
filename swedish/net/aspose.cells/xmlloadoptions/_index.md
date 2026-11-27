---
title: "Klass XmlLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.XmlLoadOptions-klass. Representerar alternativen för att läsa in XML"
type: docs
url: /sv/net/aspose.cells/xmlloadoptions/
---
## XmlLoadOptions class

Representerar alternativen för att ladda xml.

```csharp
public class XmlLoadOptions : LoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [XmlLoadOptions](xmlloadoptions/#constructor)() | Representerar alternativen för att läsa in en XML-fil. |
| [XmlLoadOptions](xmlloadoptions/#constructor_1)(LoadFormat) | Representerar alternativen för att läsa in en XML-fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Anger om data automatiskt filtreras vid inläsning av filerna.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Hämtar och anger auto‑fitter‑alternativen (Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Kontrollerar om data är giltiga i mallfilen.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32 K. När du anger ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Om du däremot har angett ett värde som är ogiltigt för Excel‑filformatet bör du inte spara arbetsboken som Excel‑format senare. Annars kan det uppstå oväntade fel i den genererade Excel‑filen.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ContainsMultipleWorksheets](../../aspose.cells/xmlloadoptions/containsmultipleworksheets/) { get; set; } | Anger om xml importeras som flera kalkylblad. |
| [ConvertNumericOrDate](../../aspose.cells/xmlloadoptions/convertnumericordate/) { get; set; } | Anger om värdet i xml-filen konverteras till numeriskt eller datum. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för den arbetsbok som ska läsas in.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DateFormat](../../aspose.cells/xmlloadoptions/dateformat/) { get; set; } | Hämtar och anger formatet för datumvärdet. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Hämtar standardstilinställningarna för att initiera stilar i arbetsboken (Inherited from [`LoadOptions`](../loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för den [`Workbook`](../workbook/) som använder dessa [`LoadOptions`](../loadoptions/) för inläsning. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignorera data som inte skrivs ut om filen skrivs ut direkt (Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreRootAttributes](../../aspose.cells/xmlloadoptions/ignorerootattributes/) { get; set; } | Anger om attribut för rot-elementet ska ignoreras. |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Anger om onödiga former ska ignoreras. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Hämtar och anger avbrottsmontorn. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [IsXmlMap](../../aspose.cells/xmlloadoptions/isxmlmap/) { get; set; } | Anger om xml ska mappas till Excel. Standardvärdet är falskt. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Om de oparserade data ska hållas i minnet för arbetsboken när den läses in från en mallfil. Standard är true. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Hämtar eller anger gränssnittsspråket för arbetsboksversionen baserat på CountryCode som sparade filen. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Datahanteraren för att bearbeta celldata när mallfilen läses. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Filtret som anger hur data ska läsas in. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Hämtar inläsningsformatet. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Hämtar eller anger minnesläget för den inlästa arbetsboken. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [NumberFormat](../../aspose.cells/xmlloadoptions/numberformat/) { get; set; } | Hämtar och anger formatet för numeriskt värde. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Anger om formeln ska parsas när filen läses. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Anger om pivottabellens cachade poster ska parsas vid inläsning av filen. Standardvärdet är false. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Hämtar och anger lösenordet för arbetsboken. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Anger om mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för den arbetsbok som ska läsas in.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Föråldrad.**) Anger standardteckensnittets namn(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Föråldrad.**) Anger standardteckensnittets storlek.(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [StartCell](../../aspose.cells/xmlloadoptions/startcell/) { get; set; } | Hämtar och anger startcellen. |
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

    public class XmlLoadOptionsDemo
    {
        public static void XmlLoadOptionsExample()
        {
            // Skapa en instans av XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Ställa in egenskaper
            options.StartCell = "A1";
            options.IsXmlMap = true;
            options.ContainsMultipleWorksheets = false;
            options.ConvertNumericOrDate = true;
            options.NumberFormat = "0.00";
            options.DateFormat = "yyyy-MM-dd";
            options.IgnoreRootAttributes = false;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = false;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter(LoadDataFilterOptions.All);
            options.LightCellsDataHandler = null; // Assuming no data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = null; // Assuming no individual font configs are set
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = false;

            // Läs in en XML-fil i en Workbook med de angivna alternativen
            Workbook workbook = new Workbook("XmlLoadOptionsExample_original.xml", options);
            workbook.DefaultStyle.Font.Name = "Arial";  
            workbook.DefaultStyle.Font.Size = 10;
            
            // Spara arbetsboken till en ny fil
            workbook.Save("XmlLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


