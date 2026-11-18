---
title: "LowCodeSaveOptionsProviderOfPlaceHolders Klass"
linktitle: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "LowCodeSaveOptionsProviderOfPlaceHolders klass. Inkapslar objektet som representerar lowcodesaveoptionsproviderofplaceholders i Go."
type: docs
weight: 200
url: /sv/go-cpp/lowcodesaveoptionsproviderofplaceholders/
---

## LowCodeSaveOptionsProviderOfPlaceHolders class

Implementering för att tillhandahålla sparaalternativ som sparar delade delar till filer och sökvägen för den resulterande filen definieras med platshållare.

```go

type LowCodeSaveOptionsProviderOfPlaceHolders struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_String](./newlowcodesaveoptionsproviderofplaceholders_string/) | Skapar en instans för att tillhandahålla sparalternativ enligt angivna mallar. |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofplaceholders_abstractlowcodesaveoptionsprovider/) | Skapas från ett föräldraobjekt. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Offset för bladets index mellan vad som används i filsökvägen och dess faktiska värde (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Förskjutning av delens index mellan vad som används i filsökvägen och dess faktiska värde (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Förskjutning av delens index mellan vad som används i filsökvägen och dess faktiska värde (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns ett blad, kommer bladindex och namn samt motsvarande prefix (SheetNamePrefix) inte att läggas till i filsökvägen. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Om bladindex eller namn alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns ett blad, kommer bladindex och namn samt motsvarande prefix (SheetNamePrefix) inte att läggas till i filsökvägen. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Om delningsdelens index alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns en delningsdel, kommer delningsdelens index och motsvarande prefix (SplitPartPrefix) inte att läggas till i filsökvägen. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Om delningsdelens index alltid ska läggas till i filsökvägen. Standardvärdet är falskt, det vill säga när det bara finns en delningsdel, kommer delningsdelens index och motsvarande prefix (SplitPartPrefix) inte att läggas till i filsökvägen. |
| [GetSheetNamePrefix](./getsheetnameprefix/) | Prefix för indexet på arbetsbladet. |
| [SetSheetNamePrefix](./setsheetnameprefix/) | Prefix för indexet på arbetsbladet. |
| [GetSheetIndexPrefix](./getsheetindexprefix/) | Prefix för indexet på arbetsbladet. |
| [SetSheetIndexPrefix](./setsheetindexprefix/) | Prefix för indexet på arbetsbladet. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Prefix för indexet på delningsdelen. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Prefix för indexet på delningsdelen. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | Mallen för att skapa en instans av sparalternativ i GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | Mallen för att skapa en instans av sparalternativ i GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | Hämtar sparalternativen som används för att få utdatainställningarna för den aktuella delade delen. |
| [Finish](./finish/) | Frigör resurser efter bearbetning av den aktuella delade delen. |
