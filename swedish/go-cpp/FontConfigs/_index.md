---
title: "FontConfigs-klass"
linktitle: "FontConfigs"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "FontConfigs-klass. Inkapslar objektet som representerar fontconfigs i Go."
type: docs
weight: 200
url: /sv/go-cpp/fontconfigs/
---

## FontConfigs class

Specificerar teckensnittinställningar

```go

type FontConfigs struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewFontConfigs](./newfontconfigs/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [FontConfigs_IsFontAvailable](./fontconfigs_isfontavailable/) | Indikerar om teckensnittet är tillgängligt. |
| [FontConfigs_GetFontFileDataInfo](./fontconfigs_getfontfiledatainfo/) | Hämta datainformation för teckensnittsfilens data. |
| [FontConfigs_GetDefaultFontName](./fontconfigs_getdefaultfontname/) | Hämtar eller anger standardnamnet för teckensnittet. |
| [FontConfigs_SetDefaultFontName](./fontconfigs_setdefaultfontname/) | Hämtar eller anger standardnamnet för teckensnittet. |
| [FontConfigs_GetPreferSystemFontSubstitutes](./fontconfigs_getprefersystemfontsubstitutes/) | Indikerar om systemets teckensnittssubstitut ska användas först eller inte när ett teckensnitt inte finns tillgängligt och substitutet för detta teckensnitt inte är angivet. Till exempel på Ubuntu ersätts teckensnittet \"Arial\" vanligtvis av \"Liberation Sans\". Standardvärdet är falskt. |
| [FontConfigs_SetPreferSystemFontSubstitutes](./fontconfigs_setprefersystemfontsubstitutes/) | Indikerar om systemets teckensnittssubstitut ska användas först eller inte när ett teckensnitt inte finns tillgängligt och substitutet för detta teckensnitt inte är angivet. Till exempel på Ubuntu ersätts teckensnittet \"Arial\" vanligtvis av \"Liberation Sans\". Standardvärdet är falskt. |
| [FontConfigs_SetFontSubstitutes](./fontconfigs_setfontsubstitutes/) | Teckensnittssubstitutnamn för angivet ursprungligt teckensnitt. |
| [FontConfigs_GetFontSubstitutes](./fontconfigs_getfontsubstitutes/) | Returnerar en array som innehåller teckensnittssubstitutnamn att använda om det ursprungliga teckensnittet inte finns. |
| [FontConfigs_SetFontFolder](./fontconfigs_setfontfolder/) | Anger teckensnittsmappen |
| [FontConfigs_SetFontFolders](./fontconfigs_setfontfolders/) | Anger teckensnittsmappen |
| [FontConfigs_SetFontSources](./fontconfigs_setfontsources/) | Anger teckensnittskällorna. |
| [FontConfigs_GetFontSources](./fontconfigs_getfontsources/) | Hämtar en kopia av arrayen som innehåller listan över källor |
