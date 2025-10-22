##Class Config
Aspose.Cells.AI.Config class. Represents all the settings for Cells AI
## Config class
Represents all the settings for Cells AI
```csharp
public class Config
```
## Constructors
| Name | Description |
| --- | --- |
| [Config](config/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| static [Model](../../aspose.cells.ai/config/model/) { get; set; } | The AI Model to use |
## Fields
| Name | Description |
| --- | --- |
| static [ContentChunkSize](../../aspose.cells.ai/config/contentchunksize/) | The content chunk size in the message list for the AI per request |
| static [InitialFailRetryDelay](../../aspose.cells.ai/config/initialfailretrydelay/) | The initial delay time (ms) for start a new request after a fail call |
| static [Locale](../../aspose.cells.ai/config/locale/) | The preferred language for the user locale "ar", for: "Arabic (العربية)" "bg", for: "Bulgarian (Български)" "ca", for: "Catalan (Català)" "cs", for: "Czech (Čeština)" "da", for: "Danish (Dansk)" "de", for: "German (Deutsch)" "el", for: "Greek (Ελληνικά)" "en", for: "English (English)" "es", for: "Spanish (Español)" "fa", for: "Persian (فارسی)" "fr", for: "French (Français)" "he", for: "Hebrew (עִبرִית)" "hi", for: "Hindi (हिन्दी)" "hr", for: "Croatian (Hrvatski)" "hu", for: "Hungarian (Magyar)" "id", for: "Indonesian (Indonesia)" "it", for: "Italian (Italiano)" "ja", for: "Japanese (日本語)" "ka", for: "Georgian (ქართული)" "ko", for: "Korean (한국어)" "lt", for: "Lithuanian (Lietuvis)" "ms", for: "Malay (Bahasa Melayu)" "nl", for: "Dutch (Nederlands)" "pl", for: "Polish (Polskie)" "pt", for: "Portuguese (Português)" "ro", for: "Romanian (Română)" "ru", for: "Russian (Русский)" "sk", for: "Slovak (Slovák)" "th", for: "Thai (ภาษาไทย)" "tr", for: "Turkish (Türk)" "uk", for: "Ukrainian (Український)" "vi", for: "Vietnamese (Tiếng Việt)" "zh", for: "Simplified Chinese (简体中文)" "zh-hant", for: "Traditional Chinese (繁體中文)" |
| static [LogDirectory](../../aspose.cells.ai/config/logdirectory/) | The log file directory |
| static [LogLevel](../../aspose.cells.ai/config/loglevel/) | whether to add log |
| static [MaxRetryTimes](../../aspose.cells.ai/config/maxretrytimes/) | The maximum retry times for getting a response from AI ,if fail will start a new request. |
| static [MaxTokens](../../aspose.cells.ai/config/maxtokens/) | The max token number for the AI per request |
| static [Temperature](../../aspose.cells.ai/config/temperature/) | The default AI Temperature to use, When Temperature approaches 0, the model's choices become very deterministic, almost always selecting the output with the highest probability. When Temperature approaches 1 or higher, the model's outputs become more random and diversified. |
| static [TimeOutSeconds](../../aspose.cells.ai/config/timeoutseconds/) | The time out seconds for the AI to respond |
### See Also
* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [CellsAI](../../)
