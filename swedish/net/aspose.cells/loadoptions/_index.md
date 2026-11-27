---
title: "Klass LoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LoadOptions-klass. Representerar alternativ för att ladda filen"
type: docs
url: /sv/net/aspose.cells/loadoptions/
---
## LoadOptions class

Representerar alternativen för att läsa in filen.

```csharp
public class LoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LoadOptions](loadoptions/#constructor)() | Skapar alternativ för att läsa in filen. |
| [LoadOptions](loadoptions/#constructor_1)(LoadFormat) | Skapar alternativ för att läsa in filen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Indikerar om data automatiskt filtreras vid inläsning av filerna. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Hämtar och anger alternativen för automatisk anpassning |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Kontrollera om data är giltiga i mallfilen. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att en strängvärde längre än 32 K matas in. När du matar in ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för Workbook som ska laddas. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Hämtar standardinställningarna för stil vid initiering av arbetsbokens stilar. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för den [`Workbook`](../workbook/) som använder detta `LoadOptions` för att laddas. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignorera data som inte skrivs ut om filen skrivs ut direkt. |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Anger om onödiga former ska ignoreras. |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Hämtar och anger avbrottsövervakaren. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Om de oparsade data ska behållas i minnet för Workbook när den laddas från mallfilen. Standard är true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Hämtar eller anger användargränssnittsspråket för arbetsbokens version baserat på landskoden som har sparat filen. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Datahanteraren för bearbetning av celldata när mallfilen läses. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Filtret som anger hur data ska laddas. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Hämtar laddningsformatet. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Hämtar eller anger minnesläget för den laddade Workbook. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Anger om formeln ska parsas när filen läses. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Anger om pivot‑cachade poster ska parsas vid inläsning av filen. Standardvärdet är false. |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Hämtar och anger lösenordet för Workbook. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras vid hämtning och angivning av formler. Standardvärdet är false. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för Workbook som ska laddas. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Anger standardteckensnittets namn |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Anger standardteckensnittets storlek. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Hämtar eller anger varningsåteranrop. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Anger standardpappersstorlek för utskrift från standardskrivarens inställning. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class LoadOptionsDemo
    {
        public static void LoadOptionsExample()
        {
            // Skapa en instans av LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Ställa in egenskaper
            loadOptions.Password = "password123";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new CultureInfo("en-US");
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = false;
            loadOptions.KeepUnparsedData = true;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Läs in en arbetsbok med de angivna LoadOptions
            Workbook workbook = new Workbook("LoadOptionsExample_original.xlsx", loadOptions);

            // Utför operationer på Workbook
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, World!");

            // Spara arbetsboken
            workbook.Save("LoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


