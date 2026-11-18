---
title: "SpreadsheetML2003SaveOptions-klass"
linktitle: "SpreadsheetML2003SaveOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "SpreadsheetML2003SaveOptions-klass. Inkapslar objektet som representerar spreadsheetml2003saveoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/spreadsheetml2003saveoptions/
---

## SpreadsheetML2003SaveOptions class

Representerar alternativen för att spara Excel 2003 spreadml-fil.

```go

type SpreadsheetML2003SaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewSpreadsheetML2003SaveOptions](./newspreadsheetml2003saveoptions/) | Skapar alternativen för att spara Excel 2003 spreadml-fil. |
| [NewSpreadsheetML2003SaveOptions_SaveOptions](./newspreadsheetml2003saveoptions_saveoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [IsIndentedFormatting](./isindentedformatting/) | Gör att underordnade element indenteras. |
| [SetIsIndentedFormatting](./setisindentedformatting/) | Gör att underordnade element indenteras. |
| [GetLimitAsXls](./getlimitasxls/) | Begränsning för xls, det maximala radindexet är 65535 och det maximala kolumnindexet är 255. |
| [SetLimitAsXls](./setlimitasxls/) | Begränsning för xls, det maximala radindexet är 65535 och det maximala kolumnindexet är 255. |
| [GetExportColumnIndexOfCell](./getexportcolumnindexofcell/) | Standardvärdet är falskt, det betyder att kolumnindexet kommer att ignoreras om cellen är sammanhängande med föregående cell. |
| [SetExportColumnIndexOfCell](./setexportcolumnindexofcell/) | Standardvärdet är falskt, det betyder att kolumnindexet kommer att ignoreras om cellen är sammanhängande med föregående cell. |
| [GetSaveFormat](./getsaveformat/) | Hämtar formatet för sparad fil. |
| [GetClearData](./getcleardata/) | Gör arbetsboken tom efter att filen har sparats. |
| [SetClearData](./setcleardata/) | Gör arbetsboken tom efter att filen har sparats. |
| [GetCachedFileFolder](./getcachedfilefolder/) | Mappen för temporära filer som kan användas som datacache. |
| [SetCachedFileFolder](./setcachedfilefolder/) | Mappen för temporära filer som kan användas som datacache. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [GetMergeAreas](./getmergeareas/) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [SetMergeAreas](./setmergeareas/) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [GetCreateDirectory](./getcreatedirectory/) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [SetCreateDirectory](./setcreatedirectory/) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [GetSortNames](./getsortnames/) | Anger om definierade namn ska sorteras innan filen sparas. |
| [SetSortNames](./setsortnames/) | Anger om definierade namn ska sorteras innan filen sparas. |
| [GetSortExternalNames](./getsortexternalnames/) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [SetSortExternalNames](./setsortexternalnames/) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Anger om den senaste datan för diagrammet ska cachas. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Anger om den senaste datan för diagrammet ska cachas. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32K. När du matar in ett värde längre än 32K kommer det att trunkeras. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32K. När du matar in ett värde längre än 32K kommer det att trunkeras. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Anger om smart art-inställningarna ska uppdateras. Standardvärdet är false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Anger om smart art-inställningarna ska uppdateras. Standardvärdet är false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Anger om dokumentegenskaper ska krypteras när du sparar som .xls-fil. Standardvärdet är true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Anger om dokumentegenskaper ska krypteras när du sparar som .xls-fil. Standardvärdet är true. |
