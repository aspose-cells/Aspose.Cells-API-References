---
title: "LowCodeSaveOptionsProviderOfAssembling Class"
linktitle: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "LowCodeSaveOptionsProviderOfAssembling class. Incapsula l'oggetto che rappresenta lowcodesaveoptionsproviderofassembling in Go."
type: docs
weight: 200
url: /it/go-cpp/lowcodesaveoptionsproviderofassembling/
---

## LowCodeSaveOptionsProviderOfAssembling class

Implementazione per fornire opzioni di salvataggio che salvano le parti divise in file e il percorso del file risultante è denominato come (può contenere directory):<see cref="PathHeader"/>+<see cref="SheetPrefix"/>+SheetIndex(o SheetName)+<see cref="SplitPartPrefix"/>+SplitPartIndex+<see cref="PathTail"/>.

```go

type LowCodeSaveOptionsProviderOfAssembling struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfAssembling](./newlowcodesaveoptionsproviderofassembling/) | Costruttore predefinito. |
| [NewLowCodeSaveOptionsProviderOfAssembling_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofassembling_abstractlowcodesaveoptionsprovider/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetPathHeader](./getpathheader/) | Parte dell'intestazione (prima del contenuto aggiunto del foglio e della parte divisa) del percorso file. |
| [SetPathHeader](./setpathheader/) | Parte dell'intestazione (prima del contenuto aggiunto del foglio e della parte divisa) del percorso file. |
| [GetPathTail](./getpathtail/) | Parte finale (dopo i numeri di sequenza) del percorso file. Dovrebbe includere l'estensione del nome file. |
| [SetPathTail](./setpathtail/) | Parte finale (dopo i numeri di sequenza) del percorso file. Dovrebbe includere l'estensione del nome file. |
| [GetUseSheetName](./getusesheetname/) | Indica se costruire il percorso file con il nome del foglio invece dell'indice del foglio. Il valore predefinito è false. |
| [SetUseSheetName](./setusesheetname/) | Indica se costruire il percorso file con il nome del foglio invece dell'indice del foglio. Il valore predefinito è false. |
| [GetSheetPrefix](./getsheetprefix/) | Prefisso per l'indice del foglio di lavoro. |
| [SetSheetPrefix](./setsheetprefix/) | Prefisso per l'indice del foglio di lavoro. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Prefisso per l'indice della parte divisa. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Prefisso per l'indice della parte divisa. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Offset dell'indice del foglio tra quello usato nel percorso file e il suo valore reale (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Offset dell'indice del foglio tra quello usato nel percorso file e il suo valore reale (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Offset dell'indice della parte divisa tra quello usato nel percorso file e il suo valore reale (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Offset dell'indice della parte divisa tra quello usato nel percorso file e il suo valore reale (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Indica se aggiungere sempre l'indice o il nome del foglio al percorso file. Il valore predefinito è false, cioè, quando c'è un solo foglio, l'indice (o il nome) del foglio e il prefisso corrispondente non verranno aggiunti al percorso file. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Indica se aggiungere sempre l'indice o il nome del foglio al percorso file. Il valore predefinito è false, cioè, quando c'è un solo foglio, l'indice (o il nome) del foglio e il prefisso corrispondente non verranno aggiunti al percorso file. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Indica se aggiungere sempre l'indice della parte divisa al percorso file. Il valore predefinito è false, cioè, quando c'è una sola parte divisa, l'indice della parte divisa e il prefisso corrispondente non verranno aggiunti al percorso file. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Indica se aggiungere sempre l'indice della parte divisa al percorso file. Il valore predefinito è false, cioè, quando c'è una sola parte divisa, l'indice della parte divisa e il prefisso corrispondente non verranno aggiunti al percorso file. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | Il modello per creare un'istanza delle opzioni di salvataggio in GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | Il modello per creare un'istanza delle opzioni di salvataggio in GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte attualmente divisa. |
| [Finish](./finish/) | Rilascia le risorse dopo l'elaborazione della parte attualmente divisa. |
