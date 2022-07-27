---
title: GridJsWorkbook
second_title: Aspose.Cells för .NET API-referens
description: Representerar huvudinträdesklassen för GridJs
type: docs
weight: 80
url: /sv/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Representerar huvudinträdesklassen för GridJs

```csharp
public class GridJsWorkbook
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings) { get; set; } | Representerar arbetsboksinställningarna. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback) { get; set; } | Hämtar eller ställer in varningsåteruppringning för importfil. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape)(string, string) | kopiera bild eller form i kalkylbladet |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson)(string) | return error message |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson#exporttojson)() | Hämta json från workbook |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson#exporttojson_1)(string) | Hämta json från workbook |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder)(string) | Hämta json från workbook |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid)(string, string) | hämta json från cachen av uid |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_3)(string) | Importerar från en excel-fil. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile)(Workbook) | Importer från arbetsbok. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_1)(Stream, GridLoadFormat) | Importer från en excel-fil stream. måste tillhandahålla loadformat och kan ställa in GridJsWorkbook.CacheImp för att implementera stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_7)(string, string) | Importerar från en excel-fil. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_4)(string, Workbook) | Importerar från en excel-fil. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_2)(Stream, GridLoadFormat, string) | Importer från en excel-fil stream. måste tillhandahålla loadformat och kan ställa in GridJsWorkbook.CacheImp för att implementera stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_5)(string, Stream, GridLoadFormat) | Importer från en excel-fil stream. måste tillhandahålla loadformat och kan ställa in GridJsWorkbook.CacheImp för att implementera stream cache |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_8)(string, string, string) | Importerar från en excel-fil. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Importer från en excel-fil stream. måste tillhandahålla loadformat och kan ställa in GridJsWorkbook.CacheImp för att implementera stream cache |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson)(string) | Importera fil från json |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage)(string, string, Stream, string) | infoga bild i kalkylbladet |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson)(string, string) | Tillämpa stiluppdatering på cachefilen |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename)(string, string, string) | Sparar kalkylbladen i cachen, sparaformatet baseras på filtillägget för filnamnet . |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile#savetoexcelfile)(Stream) | Sparar kalkylbladen till sream, baserat på ursprungsfilformatet . |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile#savetoexcelfile_1)(string) | Sparar kalkylbladen till filsökvägen, om filen har filtillägget baseras sparaformatet på filtillägget . |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml#savetohtml)(Stream) | Sparar kalkylbladen till sream, sparaformatet är html |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml#savetohtml_1)(string) | Sparar kalkylbladen till filsökvägen, sparaformatet är html |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf#savetopdf)(Stream) | Sparar kalkylbladen till sream, sparaformatet är pdf |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf#savetopdf_1)(string) | Sparar kalkylbladen till filsökvägen, sparaformatet är pdf |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx#savetoxlsx)(Stream) | Sparar kalkylbladen till sream, sparaformatet är xlsx |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx#savetoxlsx_1)(string) | Sparar kalkylbladen till filsökvägen, sparaformatet är xlsx |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload)(GridInterruptMonitor, int) | ställ in InterruptMonitor för laddningsoperation för arbetsbok |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave)(GridInterruptMonitor) | ställ in InterruptMonitor för sparoperation för arbetsbok |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell)(string, string) | Uppdatera operation |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat)(string) | Hämta GridLoadFormat med filtillägget |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream)(string, string) | Få ström av bild från workbook |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl)(string, string, string) | Hämta bilden URL |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile)(string) | Generera uid för filen |

## Fält

| namn | Beskrivning |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp) | Anpassad implementering för cachelagring, om du vill lagra cache på stream-sätt måste du ställa in och implementera it |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine) | Anpassad implementering för beräkningsmotor ,Om du vill göra anpassad beräkning måste du ställa in och implementera it |

### Se även

* namnutrymme [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* hopsättning [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
