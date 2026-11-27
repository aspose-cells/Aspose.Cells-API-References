---
title: "Klass Config"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AI.Config klass. Representerar alla inställningar för Cells AI"
type: docs
url: /sv/net/aspose.cells.ai/config/
---
## Config class

Representerar alla inställningar för Cells AI.

```csharp
public class Config
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Config](config/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| static [Model](../../aspose.cells.ai/config/model/) { get; set; } | AI-modellen att använda |

## Fält

| Namn | Beskrivning |
| --- | --- |
| static [ContentChunkSize](../../aspose.cells.ai/config/contentchunksize/) | Storleken på innehållsdelarna i meddelandelistan för AI per begäran |
| static [InitialFailRetryDelay](../../aspose.cells.ai/config/initialfailretrydelay/) | Den initiala fördröjningstiden (ms) för att starta en ny begäran efter ett misslyckat anrop |
| static [Locale](../../aspose.cells.ai/config/locale/) | Det föredragna språket för användarens lokal "ar", för: "Arabic (العربية)" "bg", för: "Bulgarian (Български)" "ca", för: "Catalan (Català)" "cs", för: "Czech (Čeština)" "da", för: "Danish (Dansk)" "de", för: "German (Deutsch)" "el", för: "Greek (Ελληνικά)" "en", för: "English (English)" "es", för: "Spanish (Español)" "fa", för: "Persian (فارسی)" "fr", för: "French (Français)" "he", för: "Hebrew (עִברִית)" "hi", för: "Hindi (हिन्दी)" "hr", för: "Croatian (Hrvatski)" "hu", för: "Hungarian (Magyar)" "id", för: "Indonesian (Indonesia)" "it", för: "Italian (Italiano)" "ja", för: "Japanese (日本語)" "ka", för: "Georgian (ქართული)" "ko", för: "Korean (한국어)" "lt", för: "Lithuanian (Lietuvis)" "ms", för: "Malay (Bahasa Melayu)" "nl", för: "Dutch (Nederlands)" "pl", för: "Polish (Polskie)" "pt", för: "Portuguese (Português)" "ro", för: "Romanian (Română)" "ru", för: "Russian (Русский)" "sk", för: "Slovak (Slovák)" "th", för: "Thai (ภาษาไทย)" "tr", för: "Turkish (Türk)" "uk", för: "Ukrainian (Український)" "vi", för: "Vietnamese (Tiếng Việt)" "zh", för: "Simplified Chinese (简体中文)" "zh-hant", för: "Traditional Chinese (繁體中文)" |
| static [LogDirectory](../../aspose.cells.ai/config/logdirectory/) | Loggfilens katalog |
| static [LogLevel](../../aspose.cells.ai/config/loglevel/) | om logg ska läggas till |
| static [MaxRetryTimes](../../aspose.cells.ai/config/maxretrytimes/) | Det maximala antalet omförsök för att få ett svar från AI, om misslyckas startas en ny begäran. |
| static [MaxTokens](../../aspose.cells.ai/config/maxtokens/) | Det maximala antalet token för AI per begäran |
| static [Temperature](../../aspose.cells.ai/config/temperature/) | Standard AI Temperature att använda, När Temperature närmar sig 0 blir modellens val mycket deterministiska, nästan alltid väljer utdata med högst sannolikhet. När Temperature närmar sig 1 eller högre blir modellens utdata mer slumpmässiga och diversifierade. |
| static [TimeOutSeconds](../../aspose.cells.ai/config/timeoutseconds/) | Timeout‑sekunderna för AI att svara |

### Se även

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [CellsAI](../../)


