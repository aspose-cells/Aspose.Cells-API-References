---
title: "Klassen WebWorksheets"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.WebWorksheets-klass."
type: docs
url: /sv/net/aspose.cells.gridweb.data/webworksheets/
---
## WebWorksheets class

```csharp
[Obsolete("This class is obsolete; use  GridWorksheetCollection instead")]
public class WebWorksheets : ICollection, ISerializable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [WebWorksheets](webworksheets/)(MainWeb, GridWorksheetCollection) |  |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActiveSheet](../../aspose.cells.gridweb.data/webworksheets/activesheet/) { get; } |  |
| [ActiveSheetIndex](../../aspose.cells.gridweb.data/webworksheets/activesheetindex/) { get; set; } |  |
| [Count](../../aspose.cells.gridweb.data/webworksheets/count/) { get; } |  |
| [DefaultFontName](../../aspose.cells.gridweb.data/webworksheets/defaultfontname/) { get; set; } |  |
| [DefaultFontSize](../../aspose.cells.gridweb.data/webworksheets/defaultfontsize/) { get; set; } |  |
| [IsFixedSize](../../aspose.cells.gridweb.data/webworksheets/isfixedsize/) { get; } | Hämtar ett värde som indikerar om samlingen har en fast storlek. |
| [IsReadOnly](../../aspose.cells.gridweb.data/webworksheets/isreadonly/) { get; } | Hämtar ett värde som indikerar om IList är skrivskyddad. |
| [IsSynchronized](../../aspose.cells.gridweb.data/webworksheets/issynchronized/) { get; } | Hämtar ett värde som indikerar om åtkomst till ICollection är synkroniserad (trådsäker). |
| [Item](../../aspose.cells.gridweb.data/webworksheets/item/) { get; } | Hämtar Worksheet-elementet på det angivna indexet. (2 indexerare). |
| [PivotCaches](../../aspose.cells.gridweb.data/webworksheets/pivotcaches/) { get; } | Hämtar PivotCache-samlingsobjektet |
| [PivotTables](../../aspose.cells.gridweb.data/webworksheets/pivottables/) { get; } | Hämtar pivotTable-samlingsobjektet. |
| [SyncRoot](../../aspose.cells.gridweb.data/webworksheets/syncroot/) { get; } | Hämtar ett objekt som kan användas för att synkronisera åtkomst till ICollection. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add)() | Lägger till ett kalkylblad i samlingen. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_1)(object) | Lägger till ett bladobjekt. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_2)(string) | Lägger till ett kalkylblad i samlingen. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_1)(int) | Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_2)(string) | Lägger till ett arbetsblad i samlingen och kopierar data från ett befintligt arbetsblad. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy)(WebWorksheet) | Lägger till ett arbetsblad i samlingen och kopierar data från ett befintligt arbetsblad. |
| [Clear](../../aspose.cells.gridweb.data/webworksheets/clear/)() | Rensa alla arbetsblad. |
| [Contains](../../aspose.cells.gridweb.data/webworksheets/contains/)(object) | Indikerar om samlingen innehåller bladet. |
| [CopyTo](../../aspose.cells.gridweb.data/webworksheets/copyto/)(Array, int) | Kopierar innehållet till en array. |
| [GetEnumerator](../../aspose.cells.gridweb.data/webworksheets/getenumerator/)() |  |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview)(DataView, TableItemStyle, TableItemStyle) | Importerar från en DataView. Skapar automatiskt ett blad med DataView:ens tabellnamn. |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview_1)(DataView, TableItemStyle, TableItemStyle, string, int, int) | Importerar från en DataView till det angivna bladet och positionen. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile)(Stream) | Importerar från en Excel-filström, inklusive filström från disk eller minnesström. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile_1)(string) | Importerar från en Excel-fil. |
| [IndexOf](../../aspose.cells.gridweb.data/webworksheets/indexof/)(object) | Hämtar bladets index. |
| [Insert](../../aspose.cells.gridweb.data/webworksheets/insert/)(int, string) | Infogar ett blad på indexet. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile)(Stream) | Läser in data från en CSV-filström. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile_1)(string) | Läser in data från en CSV-fil. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile)(Stream) | Läser in data från en HTML-filström. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile_1)(string) | Läser in data från en HTML-fil. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Läser in data från en SpreadSheetML-filström. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Läser in data från en SpreadSheetML-fil. |
| [Remove](../../aspose.cells.gridweb.data/webworksheets/remove/)(object) | Tar bort ett blad. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat)(int) | Tar bort ett blad på indexet. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat_1)(string) | Tar bort elementet med ett angivet namn. |
| [RunAllFormulas](../../aspose.cells.gridweb.data/webworksheets/runallformulas/)() | Kör alla cellers formler. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile)(Stream) | Sparar data till en CSV-filström. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile_1)(string) | Sparar data till en CSV-fil. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile)(Stream) | Sparar data till en HTML-filström. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile_1)(string) | Sparar data till en HTML-fil. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Sparar data till en SpreadSheetML-filström. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Sparar data till en SpreadSheetML-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile)(Stream) | Sparar arbetsbladen till en excel-filström, inklusive disk‑IO‑ström eller minnesström. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_2)(string) | Sparar arbetsbladen till en excel-fil i Excel 2003-format. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Sparar arbetsbladen till en excel-fil. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_3)(string, GridSaveFormat) | Sparar arbetsbladen till en excel-fil. |

### Anmärkningar

OBS: Den här klassen är nu föråldrad. använd GridWorksheetCollection istället. Den här klassen kommer att tas bort efter 6 månader sedan augusti 2014. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


