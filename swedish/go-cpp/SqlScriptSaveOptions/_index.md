---
title: "SqlScriptSaveOptions Klass"
linktitle: "SqlScriptSaveOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "SqlScriptSaveOptions klass. Inkapslar objektet som representerar sqlscriptsaveoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

Representerar alternativen för att spara sql.

```go

type SqlScriptSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewSqlScriptSaveOptions](./newsqlscriptsaveoptions/) | Skapar alternativ för att spara sql‑fil. |
| [NewSqlScriptSaveOptions_SaveOptions](./newsqlscriptsaveoptions_saveoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetCheckIfTableExists](./getcheckiftableexists/) | Kontrollera om tabellnamnet finns innan skapande |
| [SetCheckIfTableExists](./setcheckiftableexists/) | Kontrollera om tabellnamnet finns innan skapande |
| [GetColumnTypeMap](./getcolumntypemap/) | Hämtar och sätter mappningen av kolumntyp för olika databaser. |
| [SetColumnTypeMap](./setcolumntypemap/) | Hämtar och sätter mappningen av kolumntyp för olika databaser. |
| [GetCheckAllDataForColumnType](./getcheckalldataforcolumntype/) | Kontrollera all data för att hitta kolumners datatyp. |
| [SetCheckAllDataForColumnType](./setcheckalldataforcolumntype/) | Kontrollera all data för att hitta kolumners datatyp. |
| [GetAddBlankLineBetweenRows](./getaddblanklinebetweenrows/) | Infoga en tom rad mellan varje datapost. |
| [SetAddBlankLineBetweenRows](./setaddblanklinebetweenrows/) | Infoga en tom rad mellan varje datapost. |
| [GetSeparator](./getseparator/) | Hämtar och sätter teckenseparatorn för sql‑skript. |
| [SetSeparator](./setseparator/) | Hämtar och sätter teckenseparatorn för sql‑skript. |
| [GetOperatorType](./getoperatortype/) | Hämtar och sätter operatortypen för sql. |
| [SetOperatorType](./setoperatortype/) | Hämtar och sätter operatortypen för sql. |
| [GetPrimaryKey](./getprimarykey/) | Representerar vilken kolumn som är primärnyckel i datatabellen. |
| [SetPrimaryKey](./setprimarykey/) | Representerar vilken kolumn som är primärnyckel i datatabellen. |
| [GetCreateTable](./getcreatetable/) | Anger om sql för att skapa tabell exporteras. |
| [SetCreateTable](./setcreatetable/) | Anger om sql för att skapa tabell exporteras. |
| [GetIdName](./getidname/) | Hämtar och sätter namnet på id‑kolumnen. |
| [SetIdName](./setidname/) | Hämtar och sätter namnet på id‑kolumnen. |
| [GetStartId](./getstartid/) | Hämtar och sätter start‑id. |
| [SetStartId](./setstartid/) | Hämtar och sätter start‑id. |
| [GetTableName](./gettablename/) | Hämtar och sätter tabellnamnet. |
| [SetTableName](./settablename/) | Hämtar och sätter tabellnamnet. |
| [GetExportAsString](./getexportasstring/) | Anger om all data exporteras som strängvärde. |
| [SetExportAsString](./setexportasstring/) | Anger om all data exporteras som strängvärde. |
| [GetSheetIndexes](./getsheetindexes/) | Representerar indexen för exporterade blad. |
| [SetSheetIndexes](./setsheetindexes/) | Representerar indexen för exporterade blad. |
| [GetExportArea](./getexportarea/) | Hämtar eller sätter exportintervallet. |
| [SetExportArea](./setexportarea/) | Hämtar eller sätter exportintervallet. |
| [GetHasHeaderRow](./gethasheaderrow/) | Indikerar om området innehåller rubrikrad. |
| [SetHasHeaderRow](./sethasheaderrow/) | Indikerar om området innehåller rubrikrad. |
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
