---
title: "Classe FontConfigs"
linktitle: "FontConfigs"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe FontConfigs. Incapsula l'oggetto che rappresenta fontconfigs in Go."
type: docs
weight: 200
url: /it/go-cpp/fontconfigs/
---

## FontConfigs class

Specifica le impostazioni del font

```go

type FontConfigs struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewFontConfigs](./newfontconfigs/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [FontConfigs_IsFontAvailable](./fontconfigs_isfontavailable/) | Indica se il font è disponibile. |
| [FontConfigs_GetFontFileDataInfo](./fontconfigs_getfontfiledatainfo/) | Ottieni le informazioni sui dati del file del font. |
| [FontConfigs_GetDefaultFontName](./fontconfigs_getdefaultfontname/) | Ottiene o imposta il nome del font predefinito. |
| [FontConfigs_SetDefaultFontName](./fontconfigs_setdefaultfontname/) | Ottiene o imposta il nome del font predefinito. |
| [FontConfigs_GetPreferSystemFontSubstitutes](./fontconfigs_getprefersystemfontsubstitutes/) | Indica se utilizzare prima i sostituti di font di sistema o meno quando un font non è presente e il sostituto di questo font non è impostato. Ad esempio, su Ubuntu, il font "Arial" è generalmente sostituito da "Liberation Sans". Il valore predefinito è false. |
| [FontConfigs_SetPreferSystemFontSubstitutes](./fontconfigs_setprefersystemfontsubstitutes/) | Indica se utilizzare prima i sostituti di font di sistema o meno quando un font non è presente e il sostituto di questo font non è impostato. Ad esempio, su Ubuntu, il font "Arial" è generalmente sostituito da "Liberation Sans". Il valore predefinito è false. |
| [FontConfigs_SetFontSubstitutes](./fontconfigs_setfontsubstitutes/) | Nomi dei sostituti del font per il nome del font originale fornito. |
| [FontConfigs_GetFontSubstitutes](./fontconfigs_getfontsubstitutes/) | Restituisce un array contenente i nomi dei sostituti del font da utilizzare se il font originale non è presente. |
| [FontConfigs_SetFontFolder](./fontconfigs_setfontfolder/) | Imposta la cartella dei font |
| [FontConfigs_SetFontFolders](./fontconfigs_setfontfolders/) | Imposta la cartella dei font |
| [FontConfigs_SetFontSources](./fontconfigs_setfontsources/) | Imposta le sorgenti dei font. |
| [FontConfigs_GetFontSources](./fontconfigs_getfontsources/) | Ottiene una copia dell'array che contiene l'elenco delle sorgenti |
