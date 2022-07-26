---
title: AbstractTextLoadOptions
second_title: Aspose.Cells för .NET API-referens
description: Vanliga alternativ för att ladda textvärden
type: docs
weight: 60
url: /sv/net/aspose.cells/abstracttextloadoptions/
---
## AbstractTextLoadOptions class

Vanliga alternativ för att ladda textvärden

```csharp
public class AbstractTextLoadOptions : LoadOptions
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Indikerar om data filtreras automatiskt när filerna laddas. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Hämtar och ställer in alternativen för automatisk montering |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Kontrollera om data är giltig i mallfilen. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Om kontrollera begränsningen av excel-fil när användaren ändrar cellrelaterade objekt. Till exempel tillåter excel inte inmatning av strängvärden som är längre än 32K. När du matar in ett värde längre än 32K såsom av Cell.PutValue(sträng), om detta egenskapen är sant får du ett undantag. Om den här egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan mata ut hela strängvärdet för andra filformat som CSV. Men om du har angett ett sådant värde som är ogiltigt för Excel-filformat, du bör inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå ett oväntat fel för den genererade excel-filen. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Hämtar eller ställer in ett värde som indikerar om strängen i textfilen konverteras till datumdata. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Hämtar eller ställer in ett värde som indikerar om strängen i textfilen konverteras till numerisk data. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Hämtar eller ställer in systemkulturinformationen vid den tidpunkt då filen laddades. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Hämtar standardstilsinställningarna för att initiera stilar för arbetsboken |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Hämtar och ställer in standardkodningen. Gäller endast för csv-fil. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Hämtar och ställer in individuella teckensnittskonfigurationer. Fungerar bara för[`Workbook`](../workbook) som använder detta[`LoadOptions`](../loadoptions) att ladda.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignorera data som inte skrivs ut om du skriver ut filen direkt |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Hämtar och ställer in avbrottsmonitorn. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Anger om ett strängvärde inte analyseras om längden är 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Behåller den oparsade datan i minnet för arbetsboken när den laddas från mallfilen. Standard är sant. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Hämtar eller ställer in användargränssnittsspråket för versionen av arbetsboken baserat på CountryCode som har sparat filen. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Datahanteraren för att bearbeta celldata vid läsning av mallfil. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Filtret för att ange hur man laddar data. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Hämtar laddningsformatet. |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Indikerar strategin för att tillämpa stil för analyserade värden vid konvertering av strängvärde till nummer eller datetime. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Hämtar eller ställer in minnesanvändningsalternativen. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Indikerar om formeln analyseras när filen läses. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Indikerar om tolkning av pivotcachade poster när filen laddas. Standardvärdet är false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Hämtar och ställer in lösenordet för arbetsboken. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Hämtar eller ställer in systemets regionala inställningar baserat på CountryCode vid den tidpunkt då filen laddades. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Får eller ställer in varningsåteruppringning. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Ställer in standardstorleken för utskriftspapper från standardskrivarens inställning. |

### Se även

* class [LoadOptions](../loadoptions)
* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
