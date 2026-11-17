---
title: "LowCodeSaveOptionsProviderOfPlaceHolders Classe"
linktitle: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "LowCodeSaveOptionsProviderOfPlaceHolders classe. Incapsula l'oggetto che rappresenta lowcodesaveoptionsproviderofplaceholders in Go."
type: docs
weight: 200
url: /it/go-cpp/lowcodesaveoptionsproviderofplaceholders/
---

## LowCodeSaveOptionsProviderOfPlaceHolders class

Implementazione per fornire opzioni di salvataggio che salvano le parti divise in file e il percorso del file risultante è definito con segnaposti.

```go

type LowCodeSaveOptionsProviderOfPlaceHolders struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_String](./newlowcodesaveoptionsproviderofplaceholders_string/) | Istanzia un'istanza per fornire le opzioni di salvataggio secondo i modelli specificati. |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofplaceholders_abstractlowcodesaveoptionsprovider/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Offset dell'indice del foglio tra quello usato nel percorso file e il suo valore reale (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Offset dell'indice del foglio tra quello usato nel percorso file e il suo valore reale (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Offset dell'indice della parte divisa tra quello usato nel percorso file e il suo valore reale (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Offset dell'indice della parte divisa tra quello usato nel percorso file e il suo valore reale (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Indica se aggiungere sempre l'indice o il nome del foglio al percorso del file. Il valore predefinito è false, cioè, quando c'è un solo foglio, l'indice e il nome del foglio e il prefisso corrispondente (SheetNamePrefix) non verranno aggiunti al percorso del file. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Indica se aggiungere sempre l'indice o il nome del foglio al percorso del file. Il valore predefinito è false, cioè, quando c'è un solo foglio, l'indice e il nome del foglio e il prefisso corrispondente (SheetNamePrefix) non verranno aggiunti al percorso del file. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Indica se aggiungere sempre l'indice della parte divisa al percorso del file. Il valore predefinito è false, cioè, quando c'è una sola parte divisa, l'indice della parte divisa e il prefisso corrispondente (SplitPartPrefix) non verranno aggiunti al percorso del file. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Indica se aggiungere sempre l'indice della parte divisa al percorso del file. Il valore predefinito è false, cioè, quando c'è una sola parte divisa, l'indice della parte divisa e il prefisso corrispondente (SplitPartPrefix) non verranno aggiunti al percorso del file. |
| [GetSheetNamePrefix](./getsheetnameprefix/) | Prefisso per l'indice del foglio di lavoro. |
| [SetSheetNamePrefix](./setsheetnameprefix/) | Prefisso per l'indice del foglio di lavoro. |
| [GetSheetIndexPrefix](./getsheetindexprefix/) | Prefisso per l'indice del foglio di lavoro. |
| [SetSheetIndexPrefix](./setsheetindexprefix/) | Prefisso per l'indice del foglio di lavoro. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Prefisso per l'indice della parte divisa. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Prefisso per l'indice della parte divisa. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | Il modello per creare un'istanza delle opzioni di salvataggio in GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | Il modello per creare un'istanza delle opzioni di salvataggio in GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte attualmente divisa. |
| [Finish](./finish/) | Rilascia le risorse dopo l'elaborazione della parte attualmente divisa. |
