---
title: "Klass DifLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Loading.DifLoadOptions‑klass. Representerar alternativ för inläsning av .dif‑fil"
type: docs
url: /sv/net/aspose.cells.loading/difloadoptions/
---
## DifLoadOptions class

Representerar alternativen för att ladda .dif-fil.

```csharp
public class DifLoadOptions : LoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [DifLoadOptions](difloadoptions/)() | Alternativen. |

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
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Hämtar eller anger minnesläget för laddad workbook.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Anger om formeln ska parsas när filen läses.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Anger om pivot-cachade poster ska parsas när filen laddas. Standardvärdet är false.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Hämtar och anger lösenordet för workbooken.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras vid hämtning och angivning av formler. Standardvärdet är false.(ärvd från [`LoadOptions`](../../aspose.cells/loadoptions/).) |
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
    using Aspose.Cells.Loading;

    public class LoadingClassDifLoadOptionsDemo
    {
        public static void Run()
        {
            // Skapa DifLoadOptions‑instans
            DifLoadOptions loadOptions = new DifLoadOptions();

            // Skapa en workbook (med parameterlös konstruktor)
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange några exempeldata
            worksheet.Cells["A1"].PutValue("Sample DIF Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Beräkna formler om några finns
            workbook.CalculateFormula();

            // Spara arbetsboken i DIF-format
            workbook.Save("DifLoadOptionsOutput.dif", SaveFormat.Dif);

            // Visa nu hur man laddar DIF-filen med DifLoadOptions
            DifLoadOptions difOptions = new DifLoadOptions();
            
            // Läs in den sparade DIF-filen med alternativen
            Workbook loadedWorkbook = new Workbook("DifLoadOptionsOutput.dif", difOptions);

            // Åtkomst till data från den inlästa arbetsboken
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            string loadedValue = loadedWorksheet.Cells["A1"].StringValue;

            // Spara den inlästa datan till XLSX för verifiering
            loadedWorkbook.Save("DifLoadOptionsVerification.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Loading](../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../)


