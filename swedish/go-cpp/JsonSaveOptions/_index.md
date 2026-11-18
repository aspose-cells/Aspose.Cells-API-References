---
title: "JsonSaveOptions-klass"
linktitle: "JsonSaveOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "JsonSaveOptions-klass. Inkapslar objektet som representerar jsonsaveoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/jsonsaveoptions/
---

## JsonSaveOptions class

Representerar alternativen för att spara arbetsboken som en JSON-fil.

```go

type JsonSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewJsonSaveOptions](./newjsonsaveoptions/) | Skapar alternativ för att spara json-fil. |
| [NewJsonSaveOptions_SaveOptions](./newjsonsaveoptions_saveoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetExportStylePool](./getexportstylepool/) | Anger om stilar ska exporteras kollektivt eller individuellt till varje cell. |
| [SetExportStylePool](./setexportstylepool/) | Anger om stilar ska exporteras kollektivt eller individuellt till varje cell. |
| [GetExportHyperlinkType](./getexporthyperlinktype/) | Representerar typen av export av hyperlänk till json. |
| [SetExportHyperlinkType](./setexporthyperlinktype/) | Representerar typen av export av hyperlänk till json. |
| [GetSkipEmptyRows](./getskipemptyrows/) | Anger om tomma rader ska hoppas över. |
| [SetSkipEmptyRows](./setskipemptyrows/) | Anger om tomma rader ska hoppas över. |
| [GetSheetIndexes](./getsheetindexes/) | Representerar indexen för exporterade blad. |
| [SetSheetIndexes](./setsheetindexes/) | Representerar indexen för exporterade blad. |
| [GetSchemas](./getschemas/) | Det ursprungliga json-schemat för varje kalkylblad. |
| [SetSchemas](./setschemas/) | Det ursprungliga json-schemat för varje kalkylblad. |
| [GetExportArea](./getexportarea/) | Hämtar eller sätter exportintervallet. |
| [SetExportArea](./setexportarea/) | Hämtar eller sätter exportintervallet. |
| [GetHasHeaderRow](./gethasheaderrow/) | Indikerar om området innehåller rubrikrad. |
| [SetHasHeaderRow](./sethasheaderrow/) | Indikerar om området innehåller rubrikrad. |
| [GetExportAsString](./getexportasstring/) | Exporterar cellernas strängvärde till json. |
| [SetExportAsString](./setexportasstring/) | Exporterar cellernas strängvärde till json. |
| [GetIndent](./getindent/) | Anger indraget. |
| [SetIndent](./setindent/) | Anger indraget. |
| [GetExportNestedStructure](./getexportnestedstructure/) | Exporteras som föräldra-barn hierarkisk Json-struktur. |
| [SetExportNestedStructure](./setexportnestedstructure/) | Exporteras som föräldra-barn hierarkisk Json-struktur. |
| [GetExportEmptyCells](./getexportemptycells/) | Anger om tomma celler ska exporteras som null. |
| [SetExportEmptyCells](./setexportemptycells/) | Anger om tomma celler ska exporteras som null. |
| [GetAlwaysExportAsJsonObject](./getalwaysexportasjsonobject/) | Anger om Excel alltid ska exporteras till json som objekt, även om det bara finns ett kalkylblad i filen. |
| [SetAlwaysExportAsJsonObject](./setalwaysexportasjsonobject/) | Anger om Excel alltid ska exporteras till json som objekt, även om det bara finns ett kalkylblad i filen. |
| [GetToExcelStruct](./gettoexcelstruct/) | Anger om konvertering till json-struktur för Excel-filen. |
| [SetToExcelStruct](./settoexcelstruct/) | Anger om konvertering till json-struktur för Excel-filen. |
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
