---
title: "DifSaveOptions-klass"
linktitle: "DifSaveOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DifSaveOptions-klass. Inkapslar objektet som representerar difsaveoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/difsaveoptions/
---

## DifSaveOptions class

Representerar alternativen för att spara dif‑fil.

```go

type DifSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewDifSaveOptions](./newdifsaveoptions/) | Skapar alternativen för att spara DIF-fil. |
| [NewDifSaveOptions_SaveOptions](./newdifsaveoptions_saveoptions/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
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
