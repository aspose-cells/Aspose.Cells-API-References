---
title: "Klasse Config"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AI.Config-Klasse. Stellt alle Einstellungen für Cells AI dar."
type: docs
url: /de/net/aspose.cells.ai/config/
---
## Config class

Stellt alle Einstellungen für Cells AI dar.

```csharp
public class Config
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Config](config/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [Model](../../aspose.cells.ai/config/model/) { get; set; } | Das zu verwendende KI-Modell |

## Felder

| Name | Beschreibung |
| --- | --- |
| static [ContentChunkSize](../../aspose.cells.ai/config/contentchunksize/) | Die Größe des Inhaltschunks in der Nachrichtenliste für die KI pro Anfrage |
| static [InitialFailRetryDelay](../../aspose.cells.ai/config/initialfailretrydelay/) | Die anfängliche Verzögerungszeit (ms) für den Start einer neuen Anfrage nach einem fehlgeschlagenen Aufruf |
| static [Locale](../../aspose.cells.ai/config/locale/) | Die bevorzugte Sprache für das Benutzer-Locale "ar", für: "Arabic (العربية)" "bg", für: "Bulgarian (Български)" "ca", für: "Catalan (Català)" "cs", für: "Czech (Čeština)" "da", für: "Danish (Dansk)" "de", für: "German (Deutsch)" "el", für: "Greek (Ελληνικά)" "en", für: "English (English)" "es", für: "Spanish (Español)" "fa", für: "Persian (فارسی)" "fr", für: "French (Français)" "he", für: "Hebrew (עִברִית)" "hi", für: "Hindi (हिन्दी)" "hr", für: "Croatian (Hrvatski)" "hu", für: "Hungarian (Magyar)" "id", für: "Indonesian (Indonesia)" "it", für: "Italian (Italiano)" "ja", für: "Japanese (日本語)" "ka", für: "Georgian (ქართული)" "ko", für: "Korean (한국어)" "lt", für: "Lithuanian (Lietuvis)" "ms", für: "Malay (Bahasa Melayu)" "nl", für: "Dutch (Nederlands)" "pl", für: "Polish (Polskie)" "pt", für: "Portuguese (Português)" "ro", für: "Romanian (Română)" "ru", für: "Russian (Русский)" "sk", für: "Slovak (Slovák)" "th", für: "Thai (ภาษาไทย)" "tr", für: "Turkish (Türk)" "uk", für: "Ukrainian (Український)" "vi", für: "Vietnamese (Tiếng Việt)" "zh", für: "Simplified Chinese (简体中文)" "zh-hant", für: "Traditional Chinese (繁體中文)" |
| static [LogDirectory](../../aspose.cells.ai/config/logdirectory/) | Das Verzeichnis der Protokolldatei |
| static [LogLevel](../../aspose.cells.ai/config/loglevel/) | ob ein Protokoll hinzugefügt werden soll |
| static [MaxRetryTimes](../../aspose.cells.ai/config/maxretrytimes/) | Die maximale Anzahl von Wiederholungsversuchen, um eine Antwort von der KI zu erhalten; bei Fehlschlag wird eine neue Anfrage gestartet. |
| static [MaxTokens](../../aspose.cells.ai/config/maxtokens/) | Die maximale Token-Anzahl für die KI pro Anfrage |
| static [Temperature](../../aspose.cells.ai/config/temperature/) | Die standardmäßige KI-Temperatur, die verwendet wird. Wenn die Temperatur gegen 0 geht, werden die Modellentscheidungen sehr deterministisch und wählen fast immer die Ausgabe mit der höchsten Wahrscheinlichkeit. Wenn die Temperatur gegen 1 oder höher geht, werden die Modellausgaben zufälliger und vielfältiger. |
| static [TimeOutSeconds](../../aspose.cells.ai/config/timeoutseconds/) | Die Timeout‑Sekunden, bis die KI antwortet |

### Siehe auch

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [CellsAI](../../)


