---
title: "Klass TxtLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TxtLoadOptions-klass. Representerar alternativen för att läsa in textfil"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

Representerar alternativen för att läsa in en textfil.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [TxtLoadOptions](txtloadoptions/#constructor)() | Skapar alternativen för att läsa in textfil. |
| [TxtLoadOptions](txtloadoptions/#constructor_1)(LoadFormat) | Skapar alternativen för att läsa in textfil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Anger om data automatiskt filtreras vid inläsning av filerna.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Hämtar och anger auto‑fitter‑alternativen (Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Kontrollerar om data är giltiga i mallfilen.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32 K. När du anger ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Om du däremot har angett ett värde som är ogiltigt för Excel‑filformatet bör du inte spara arbetsboken som Excel‑format senare. Annars kan det uppstå oväntade fel i den genererade Excel‑filen.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till datumdata. Standardvärdet är true.(Ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till numerisk data. Standardvärdet är true.(Ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för den arbetsbok som ska läsas in.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Hämtar standardstilinställningarna för att initiera stilar i arbetsboken (Inherited from [`LoadOptions`](../loadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Hämtar och anger standardkodningen. Gäller endast för csv-filer. (ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet/) { get; set; } | Om data utökas till nästa blad när rader eller kolumner överskrider gränsen. Standard är falskt. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för den [`Workbook`](../workbook/) som använder dessa [`LoadOptions`](../loadoptions/) för inläsning. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula/) { get; set; } | Anger om texten är en formel om den börjar med "=". |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier/) { get; set; } | Om det finns textavgränsare för cellvärde. Standard är sant. |
| [HeaderColumnsCount](../../aspose.cells/txtloadoptions/headercolumnscount/) { get; set; } | Antalet rubrikkolumner som ska upprepas för utökade blad. |
| [HeaderRowsCount](../../aspose.cells/txtloadoptions/headerrowscount/) { get; set; } | Antalet rubrikrader som ska upprepas för utökade blad. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignorera data som inte skrivs ut om filen skrivs ut direkt (Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Anger om onödiga former ska ignoreras. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Hämtar och anger avbrottsmontorn. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded/) { get; set; } | Sant betyder att filen innehåller flera kodningar. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Anger om en strängvärde inte ska parsas om längden är 15. (ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Om de oparserade data ska hållas i minnet för arbetsboken när den läses in från en mallfil. Standard är true. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Hämtar eller anger gränssnittsspråket för arbetsboksversionen baserat på CountryCode som sparade filen. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Datahanteraren för att bearbeta celldata när mallfilen läses. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Filtret som anger hur data ska läsas in. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Hämtar inläsningsformatet. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Anger strategin för att tillämpa stil på parsade värden när en strängvärde konverteras till nummer eller datum/tid. (ärvd från [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MaxColumnCount](../../aspose.cells/txtloadoptions/maxcolumncount/) { get; set; } | Det maximala antalet kolumner som ska importeras för ett blad. |
| [MaxRowCount](../../aspose.cells/txtloadoptions/maxrowcount/) { get; set; } | Det maximala antalet rader som ska importeras för ett blad. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Hämtar eller anger minnesläget för den inlästa arbetsboken. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Anger om formeln ska parsas när filen läses. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Anger om pivottabellens cachade poster ska parsas vid inläsning av filen. Standardvärdet är false. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Hämtar och anger lösenordet för arbetsboken. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers/) { get; set; } | Hämtar och anger föredragna värde‑tolkare för att läsa in textfil. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Anger om mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för den arbetsbok som ska läsas in.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Separator](../../aspose.cells/txtloadoptions/separator/) { get; set; } | Hämtar och anger teckenseparator för textfil. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring/) { get; set; } | Hämtar och anger ett strängvärde som avgränsare. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Föråldrad.**) Anger standardteckensnittets namn(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Föråldrad.**) Anger standardteckensnittets storlek.(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier/) { get; set; } | Anger textavgränsaren för cellvärden. Standardavgränsaren är '\"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Om på varandra följande avgränsare ska behandlas som en. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue/) { get; set; } | Indikerar om det inledande enkelfnuttstecknet ska tas med som en del av värdet i en cell. Standard är true. Om det är false kommer det inledande enkelfnuttstecknet att tas bort från motsvarande cells värde och [`QuotePrefix`](../style/quoteprefix/) kommer att sättas till true för cellen. |
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
    using System.Text;

    public class TxtLoadOptionsDemo
    {
        public static void TxtLoadOptionsExample()
        {
            // Skapa en instans av TxtLoadOptions
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                SeparatorString = ",",
                IsMultiEncoded = false,
                HasFormula = true,
                HasTextQualifier = true,
                TextQualifier = '\"',
                TreatConsecutiveDelimitersAsOne = true,
                TreatQuotePrefixAsValue = true,
                ExtendToNextSheet = false,
                HeaderRowsCount = 1,
                HeaderColumnsCount = 1,
                MaxRowCount = 1000,
                MaxColumnCount = 50,
                Encoding = Encoding.UTF8,
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn,
                ConvertNumericData = true,
                ConvertDateTimeData = true,
                KeepPrecision = true,
                Password = "password",
                ParsingFormulaOnOpen = true,
                ParsingPivotCachedRecords = true,
                LanguageCode = CountryCode.USA,
                Region = CountryCode.USA,
                CultureInfo = new System.Globalization.CultureInfo("en-US"),
                StandardFont = "Arial",
                StandardFontSize = 10.5,
                InterruptMonitor = new InterruptMonitor(),
                IgnoreNotPrinted = true,
                CheckDataValid = true,
                CheckExcelRestriction = true,
                KeepUnparsedData = true,
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
                LightCellsDataHandler = new LightCellsDataHandler(),
                MemorySetting = MemorySetting.MemoryPreference,
                WarningCallback = new WarningCallback(),
                AutoFitterOptions = new AutoFitterOptions(),
                AutoFilter = true,
                FontConfigs = new IndividualFontConfigs(),
                IgnoreUselessShapes = true,
                PreservePaddingSpacesInFormula = true
            };

            // Läs in en CSV-fil med de angivna alternativen
            Workbook workbook = new Workbook("TxtLoadOptionsExample_original.csv", loadOptions);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("TxtLoadOptionsExample.xlsx");

            return;
        }
    }

    // Dummy-implementationer för refererade klasser/gränssnitt
    public class InterruptMonitor : AbstractInterruptMonitor
    {
        public override bool IsInterruptionRequested => false;
    }

    public class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine(warningInfo.Description);
        }
    }

    public class LightCellsDataHandler : Aspose.Cells.LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet) => true;
        public bool StartRow(int rowIndex) => true;
        public bool ProcessRow(Row row) => true;
        public bool StartCell(int columnIndex) => true;
        public bool ProcessCell(Cell cell) => true;
    }
}
```

### Se även

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


