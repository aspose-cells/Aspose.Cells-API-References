---
title: "LowCodeSaveOptionsProviderOfAssembling klass"
linktitle: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "LowCodeSaveOptionsProviderOfAssembling klass. Inkapslar objektet som representerar lowcodesaveoptionsproviderofassembling i Go."
type: docs
weight: 200
url: /sv/go-cpp/lowcodesaveoptionsproviderofassembling/
---

## LowCodeSaveOptionsProviderOfAssembling class

Implementering för att tillhandahålla sparaalternativ som sparar delade delar till filer och sökvägen för den resulterande filen namnges som (det kan innehålla kataloger):<see cref="PathHeader"/>+<see cref="SheetPrefix"/>+SheetIndex(eller SheetName)+<see cref="SplitPartPrefix"/>+SplitPartIndex+<see cref="PathTail"/>.

```go

type LowCodeSaveOptionsProviderOfAssembling struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfAssembling](./newlowcodesaveoptionsproviderofassembling/) | Standardkonstruktor. |
| [NewLowCodeSaveOptionsProviderOfAssembling_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofassembling_abstractlowcodesaveoptionsprovider/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetPathHeader](./getpathheader/) | Headerdel (före tillagt innehåll av blad och delningsdel) av filsökväg. |
| [SetPathHeader](./setpathheader/) | Headerdel (före tillagt innehåll av blad och delningsdel) av filsökväg. |
| [GetPathTail](./getpathtail/) | Slutdel (efter sekvensnummer) av filsökväg. Den bör inkludera filnamnets filändelse. |
| [SetPathTail](./setpathtail/) | Slutdel (efter sekvensnummer) av filsökväg. Den bör inkludera filnamnets filändelse. |
| [GetUseSheetName](./getusesheetname/) | Om filsökvägen byggs med bladnamn istället för bladindex. Standardvärdet är falskt. |
| [SetUseSheetName](./setusesheetname/) | Om filsökvägen byggs med bladnamn istället för bladindex. Standardvärdet är falskt. |
| [GetSheetPrefix](./getsheetprefix/) | Prefix för indexet på arbetsbladet. |
| [SetSheetPrefix](./setsheetprefix/) | Prefix för indexet på arbetsbladet. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Prefix för indexet på delningsdelen. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Prefix för indexet på delningsdelen. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Förskjutning av delens index mellan vad som används i filsökvägen och dess faktiska värde (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Förskjutning av delens index mellan vad som används i filsökvägen och dess faktiska värde (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns ett blad, kommer bladindex (eller namn) och motsvarande prefix inte att läggas till i filsökvägen. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns ett blad, kommer bladindex (eller namn) och motsvarande prefix inte att läggas till i filsökvägen. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Om delens index alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns en del, kommer delens index och motsvarande prefix inte att läggas till i filsökvägen. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Om delens index alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns en del, kommer delens index och motsvarande prefix inte att läggas till i filsökvägen. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | Mallen för att skapa en instans av sparalternativ i GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | Mallen för att skapa en instans av sparalternativ i GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | Hämtar sparalternativen som används för att få utdatainställningarna för den aktuella delade delen. |
| [Finish](./finish/) | Frigör resurser efter bearbetning av den aktuella delade delen. |
