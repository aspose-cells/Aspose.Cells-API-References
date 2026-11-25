---
title: "Classe Config"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AI.Config. Rappresenta tutte le impostazioni per Cells AI"
type: docs
url: /it/net/aspose.cells.ai/config/
---
## Config class

Rappresenta tutte le impostazioni per Cells AI.

```csharp
public class Config
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Config](config/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [Model](../../aspose.cells.ai/config/model/) { get; set; } | Il modello AI da utilizzare |

## Campi

| Nome | Descrizione |
| --- | --- |
| static [ContentChunkSize](../../aspose.cells.ai/config/contentchunksize/) | La dimensione del blocco di contenuto nella lista dei messaggi per l'AI per richiesta |
| static [InitialFailRetryDelay](../../aspose.cells.ai/config/initialfailretrydelay/) | Il tempo di ritardo iniziale (ms) per avviare una nuova richiesta dopo una chiamata fallita |
| static [Locale](../../aspose.cells.ai/config/locale/) | La lingua preferita per la localizzazione dell'utente "ar", per: "Arabic (العربية)" "bg", per: "Bulgarian (Български)" "ca", per: "Catalan (Català)" "cs", per: "Czech (Čeština)" "da", per: "Danish (Dansk)" "de", per: "German (Deutsch)" "el", per: "Greek (Ελληνικά)" "en", per: "English (English)" "es", per: "Spanish (Español)" "fa", per: "Persian (فارسی)" "fr", per: "French (Français)" "he", per: "Hebrew (עִברִית)" "hi", per: "Hindi (हिन्दी)" "hr", per: "Croatian (Hrvatski)" "hu", per: "Hungarian (Magyar)" "id", per: "Indonesian (Indonesia)" "it", per: "Italian (Italiano)" "ja", per: "Japanese (日本語)" "ka", per: "Georgian (ქართული)" "ko", per: "Korean (한국어)" "lt", per: "Lithuanian (Lietuvis)" "ms", per: "Malay (Bahasa Melayu)" "nl", per: "Dutch (Nederlands)" "pl", per: "Polish (Polskie)" "pt", per: "Portuguese (Português)" "ro", per: "Romanian (Română)" "ru", per: "Russian (Русский)" "sk", per: "Slovak (Slovák)" "th", per: "Thai (ภาษาไทย)" "tr", per: "Turkish (Türk)" "uk", per: "Ukrainian (Український)" "vi", per: "Vietnamese (Tiếng Việt)" "zh", per: "Simplified Chinese (简体中文)" "zh-hant", per: "Traditional Chinese (繁體中文)" |
| static [LogDirectory](../../aspose.cells.ai/config/logdirectory/) | La directory del file di log |
| static [LogLevel](../../aspose.cells.ai/config/loglevel/) | se aggiungere il log |
| static [MaxRetryTimes](../../aspose.cells.ai/config/maxretrytimes/) | Il numero massimo di tentativi per ottenere una risposta dall'AI, se fallisce avvierà una nuova richiesta. |
| static [MaxTokens](../../aspose.cells.ai/config/maxtokens/) | Il numero massimo di token per l'AI per richiesta |
| static [Temperature](../../aspose.cells.ai/config/temperature/) | La temperatura AI predefinita da utilizzare. Quando la Temperatura si avvicina a 0, le scelte del modello diventano molto deterministiche, selezionando quasi sempre l'output con la probabilità più alta. Quando la Temperatura si avvicina a 1 o più, le uscite del modello diventano più casuali e diversificate. |
| static [TimeOutSeconds](../../aspose.cells.ai/config/timeoutseconds/) | Il timeout in secondi per la risposta dell'AI |

### Vedi anche

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [CellsAI](../../)


