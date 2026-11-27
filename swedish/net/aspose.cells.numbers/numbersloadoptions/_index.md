---
title: "Klass NumbersLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Numbers.NumbersLoadOptions class. Representerar alternativen för att läsa in Apple Numbers-filer"
type: docs
url: /sv/net/aspose.cells.numbers/numbersloadoptions/
---
## NumbersLoadOptions class

Representerar alternativen för inläsning av Apple Numbers-filer.

```csharp
public class NumbersLoadOptions : LoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [NumbersLoadOptions](numbersloadoptions/)() | Konstruktor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indikerar om data automatiskt filtreras när filerna läses in.(Ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Hämtar och anger auto‑fitter‑alternativen(Ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Kontrollera om data är giltig i mallfilen.(Ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Huruvida restriktioner för Excel‑filen kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32 K. När du anger ett värde längre än 32 K, exempelvis med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan skriva ut hela strängvärdet för andra filformat som CSV. Däremot, om du har angett ett sådant värde som är ogiltigt för Excel‑filformatet, bör du inte spara arbetsboken som Excel‑filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel‑filen.(Ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för Workbook som ska laddas.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Hämtar standardstilinställningarna för att initiera stilar i workbook(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för [`Workbook`](../../aspose.cells/workbook/) som använder detta [`LoadOptions`](../../aspose.cells/loadoptions/) för att laddas.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignorera data som inte skrivs ut om filen skrivs ut direkt(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Anger om onödiga former ska ignoreras.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Hämtar och anger avbrottsövervakaren.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Om de oparsade data ska behållas i minnet för Workbook när den laddas från mallfil. Standard är true.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Hämtar eller anger gränssnittsspråket för Workbook-versionen baserat på CountryCode som har sparat filen.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Datahanteraren för att bearbeta celldata när mallfilen läses.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Filtret som anger hur data ska laddas.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Hämtar laddningsformatet.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadTableType](../../aspose.cells.numbers/numbersloadoptions/loadtabletype/) { get; set; } | Hämtar och anger typen av inläsning av flera tabeller i ett arbetsblad. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Hämtar eller anger minnesläget för laddad workbook.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Anger om formeln ska parsas när filen läses.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Anger om pivot-cachade poster ska parsas när filen laddas. Standardvärdet är false.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Hämtar och anger lösenordet för workbooken.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras vid hämtning och angivning av formler. Standardvärdet är false.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreserveTableName](../../aspose.cells.numbers/numbersloadoptions/preservetablename/) { get; set; } | Anger om tabellnamn ska bevaras vid import från Numbers. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för Workbook som ska laddas.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Anger standardteckensnittets namn(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Anger standardteckensnittets storlek.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Hämtar eller anger varningscallback.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Anger standardpappersstorlek för utskrift från standardskrivarens inställning.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Numbers;
    using System;
    using System.Globalization;

    public class NumbersLoadOptionsDemo
    {
        public static void NumbersLoadOptionsExample()
        {
            // Skapa en instans av NumbersLoadOptions
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Ställa in egenskaper
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                Password = "password123",
                ParsingFormulaOnOpen = true,
                ParsingPivotCachedRecords = false,
                LanguageCode = CountryCode.USA,
                Region = CountryCode.USA,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                StandardFontSize = 10.5,
                IgnoreNotPrinted = true,
                CheckDataValid = true,
                CheckExcelRestriction = true,
                KeepUnparsedData = true,
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
                LightCellsDataHandler = new CustomLightCellsDataHandler(),
                MemorySetting = MemorySetting.MemoryPreference,
                WarningCallback = new CustomWarningCallback(),
                AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true },
                AutoFilter = true,
                FontConfigs = new IndividualFontConfigs(),
                IgnoreUselessShapes = true,
                PreservePaddingSpacesInFormula = false
            };

            // Läs in en Numbers-fil med de angivna inläsningsalternativen
            Workbook workbook = new Workbook("NumbersLoadOptionsExample_original.numbers", loadOptions);

            // Spara arbetsboken i XLSX-format
            workbook.Save("NumbersLoadOptionsExample.xlsx");
        }
    }

    // Anpassad implementation av LightCellsDataHandler
    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool ProcessCell(Cell cell)
        {
            return true;
        }

        public bool ProcessRow(Row row)
        {
            return true;
        }

        public bool StartCell(int columnIndex)
        {
            return true;
        }

        public bool StartRow(int rowIndex)
        {
            return true;
        }

        public bool StartSheet(Worksheet sheet)
        {
            return true;
        }
    }

    // Anpassad implementation av IWarningCallback
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }
}
```

### Se även

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)


