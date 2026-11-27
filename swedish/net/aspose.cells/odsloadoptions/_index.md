---
title: "Klass OdsLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.OdsLoadOptions klass. Representerar alternativen för att läsa in en ODS-fil"
type: docs
url: /sv/net/aspose.cells/odsloadoptions/
---
## OdsLoadOptions class

Representerar alternativen för att läsa in ods-fil.

```csharp
public class OdsLoadOptions : LoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [OdsLoadOptions](odsloadoptions/#constructor)() | Representerar alternativen för att läsa in ods-fil. |
| [OdsLoadOptions](odsloadoptions/#constructor_1)(LoadFormat) | Representerar alternativen för att läsa in ods-fil. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ApplyExcelDefaultStyleToHyperlink](../../aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/) { get; set; } | Anger om standardstilen i Excel ska tillämpas på hyperlänken. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Anger om data automatiskt filtreras vid inläsning av filerna.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Hämtar och anger auto‑fitter‑alternativen (Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Kontrollerar om data är giltiga i mallfilen.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32 K. När du anger ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Om du däremot har angett ett värde som är ogiltigt för Excel‑filformatet bör du inte spara arbetsboken som Excel‑format senare. Annars kan det uppstå oväntade fel i den genererade Excel‑filen.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för den arbetsbok som ska läsas in.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Hämtar standardstilinställningarna för att initiera stilar i arbetsboken (Inherited from [`LoadOptions`](../loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för den [`Workbook`](../workbook/) som använder dessa [`LoadOptions`](../loadoptions/) för inläsning. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignorera data som inte skrivs ut om filen skrivs ut direkt (Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Anger om onödiga former ska ignoreras. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Hämtar och anger avbrottsmontorn. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [IsClassicPivotTable](../../aspose.cells/odsloadoptions/isclassicpivottable/) { get; set; } | Anger om pivottabellen är klassisk. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Om de oparserade data ska hållas i minnet för arbetsboken när den läses in från en mallfil. Standard är true. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Hämtar eller anger gränssnittsspråket för arbetsboksversionen baserat på CountryCode som sparade filen. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Datahanteraren för att bearbeta celldata när mallfilen läses. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Filtret som anger hur data ska läsas in. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Hämtar inläsningsformatet. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Hämtar eller anger minnesläget för den inlästa arbetsboken. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Anger om formeln ska parsas när filen läses. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Anger om pivottabellens cachade poster ska parsas vid inläsning av filen. Standardvärdet är false. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Hämtar och anger lösenordet för arbetsboken. (Inherited from [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Anger om mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [RefreshPivotTables](../../aspose.cells/odsloadoptions/refreshpivottables/) { get; set; } | Anger om pivottabeller ska uppdateras vid inläsning av filen. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Hämtar eller anger de regionala inställningarna som används för den arbetsbok som ska läsas in.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Föråldrad.**) Anger standardteckensnittets namn(Ärvd från [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Föråldrad.**) Anger standardteckensnittets storlek.(Ärvd från [`LoadOptions`](../loadoptions/).) |
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

    public class OdsLoadOptionsDemo
    {
        public static void OdsLoadOptionsExample()
        {
            // Skapa en instans av OdsLoadOptions
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // Ställa in egenskaper
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            loadOptions.RefreshPivotTables = true;
            loadOptions.Password = "your_password";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new System.Globalization.CultureInfo("en-US");
            loadOptions.StandardFont = "Arial";
            loadOptions.StandardFontSize = 10.5;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = true;
            loadOptions.KeepUnparsedData = true;
            loadOptions.LoadFilter = new LoadFilter(LoadDataFilterOptions.All);
            loadOptions.LightCellsDataHandler = new CustomLightCellsDataHandler();
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.WarningCallback = new CustomWarningCallback();
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.FontConfigs = new IndividualFontConfigs();
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Läs in en ODS-fil med de angivna alternativen
            Workbook workbook = new Workbook("OdsLoadOptionsExample_original.ods", loadOptions);

            // Spara arbetsboken till en ny fil
            workbook.Save("OdsLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


