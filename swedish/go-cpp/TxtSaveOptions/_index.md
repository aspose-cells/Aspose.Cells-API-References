---
title: "TxtSaveOptions-klass"
linktitle: "TxtSaveOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "TxtSaveOptions-klass. Inkapslar objektet som representerar txtsaveoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/txtsaveoptions/
---

## TxtSaveOptions class

Representerar sparalternativen för csv-/tab-avgränsad/annan textformat.

```go

type TxtSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewTxtSaveOptions](./newtxtsaveoptions/) | Skapar alternativ för att spara textfil. |
| [NewTxtSaveOptions_SaveFormat](./newtxtsaveoptions_saveformat/) | Skapar alternativ för att spara textfil. |
| [NewTxtSaveOptions_SaveOptions](./newtxtsaveoptions_saveoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetSeparator](./getseparator/) | Hämtar och anger teckenavgränsare för textfilen. |
| [SetSeparator](./setseparator/) | Hämtar och anger teckenavgränsare för textfilen. |
| [GetSeparatorString](./getseparatorstring/) | Hämtar och anger ett strängvärde som separator. |
| [SetSeparatorString](./setseparatorstring/) | Hämtar och anger ett strängvärde som separator. |
| [GetEncoding](./getencoding/) | Hämtar och anger standardkodning. |
| [SetEncoding](./setencoding/) | Hämtar och anger standardkodning. |
| [GetQuoteType](./getquotetype/) | Hämtar eller anger hur värden ska citeras i den exporterade textfilen. |
| [SetQuoteType](./setquotetype/) | Hämtar eller anger hur värden ska citeras i den exporterade textfilen. |
| [GetFormatStrategy](./getformatstrategy/) | Hämtar och anger formatstrategi när cellvärdet exporteras som sträng. |
| [SetFormatStrategy](./setformatstrategy/) | Hämtar och anger formatstrategi när cellvärdet exporteras som sträng. |
| [GetTrimLeadingBlankRowAndColumn](./gettrimleadingblankrowandcolumn/) | Anger om ledande tomma rader och kolumner ska trimmas, som i MS Excel. Standard är true. |
| [SetTrimLeadingBlankRowAndColumn](./settrimleadingblankrowandcolumn/) | Anger om ledande tomma rader och kolumner ska trimmas, som i MS Excel. Standard är true. |
| [GetTrimTailingBlankCells](./gettrimtailingblankcells/) | Anger om efterföljande tomma celler i en rad ska trimmas. Standard är false. |
| [SetTrimTailingBlankCells](./settrimtailingblankcells/) | Anger om efterföljande tomma celler i en rad ska trimmas. Standard är false. |
| [GetKeepSeparatorsForBlankRow](./getkeepseparatorsforblankrow/) | Anger om separatorer ska skrivas ut för tom rad. Standardvärdet är false, så innehållet för en tom rad blir tomt. |
| [SetKeepSeparatorsForBlankRow](./setkeepseparatorsforblankrow/) | Anger om separatorer ska skrivas ut för tom rad. Standardvärdet är false, så innehållet för en tom rad blir tomt. |
| [GetExportArea](./getexportarea/) | Området av celler som ska exporteras. |
| [SetExportArea](./setexportarea/) | Området av celler som ska exporteras. |
| [GetExportQuotePrefix](./getexportquoteprefix/) | Anger om enkelfnuttstecknet ska exporteras som en del av värdet i en cell när Style.QuotePrefix är true för den. Standard är false. |
| [SetExportQuotePrefix](./setexportquoteprefix/) | Anger om enkelfnuttstecknet ska exporteras som en del av värdet i en cell när Style.QuotePrefix är true för den. Standard är false. |
| [GetExportAllSheets](./getexportallsheets/) | Anger om alla blad ska exporteras till textfilen. Om false, exporteras endast det aktiva bladet, precis som i MS Excel. |
| [SetExportAllSheets](./setexportallsheets/) | Anger om alla blad ska exporteras till textfilen. Om false, exporteras endast det aktiva bladet, precis som i MS Excel. |
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
