---
title: "Класс Config"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.AI.Config. Представляет все настройки для Cells AI"
type: docs
url: /ru/net/aspose.cells.ai/config/
---
## Config class

Представляет все настройки для Cells AI.

```csharp
public class Config
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Config](config/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| static [Model](../../aspose.cells.ai/config/model/) { get; set; } | Модель ИИ для использования |

## Поля

| Имя | Описание |
| --- | --- |
| static [ContentChunkSize](../../aspose.cells.ai/config/contentchunksize/) | Размер фрагмента содержимого в списке сообщений для ИИ за запрос |
| static [InitialFailRetryDelay](../../aspose.cells.ai/config/initialfailretrydelay/) | Начальное время задержки (мс) перед запуском нового запроса после неудачного вызова |
| static [Locale](../../aspose.cells.ai/config/locale/) | Предпочтительный язык для пользовательской локали "ar", for: "Arabic (العربية)" "bg", for: "Bulgarian (Български)" "ca", for: "Catalan (Català)" "cs", for: "Czech (Čeština)" "da", for: "Danish (Dansk)" "de", for: "German (Deutsch)" "el", for: "Greek (Ελληνικά)" "en", for: "English (English)" "es", for: "Spanish (Español)" "fa", for: "Persian (فارسی)" "fr", for: "French (Français)" "he", for: "Hebrew (עִברִית)" "hi", for: "Hindi (हिन्दी)" "hr", for: "Croatian (Hrvatski)" "hu", for: "Hungarian (Magyar)" "id", for: "Indonesian (Indonesia)" "it", for: "Italian (Italiano)" "ja", for: "Japanese (日本語)" "ka", for: "Georgian (ქართული)" "ko", for: "Korean (한국어)" "lt", for: "Lithuanian (Lietuvis)" "ms", for: "Malay (Bahasa Melayu)" "nl", for: "Dutch (Nederlands)" "pl", for: "Polish (Polskie)" "pt", for: "Portuguese (Português)" "ro", for: "Romanian (Română)" "ru", for: "Russian (Русский)" "sk", for: "Slovak (Slovák)" "th", for: "Thai (ภาษาไทย)" "tr", for: "Turkish (Türk)" "uk", for: "Ukrainian (Український)" "vi", for: "Vietnamese (Tiếng Việt)" "zh", for: "Simplified Chinese (简体中文)" "zh-hant", for: "Traditional Chinese (繁體中文)" |
| static [LogDirectory](../../aspose.cells.ai/config/logdirectory/) | Каталог файлов журнала |
| static [LogLevel](../../aspose.cells.ai/config/loglevel/) | добавлять ли журнал |
| static [MaxRetryTimes](../../aspose.cells.ai/config/maxretrytimes/) | Максимальное количество повторных попыток получения ответа от ИИ, при неудаче будет начат новый запрос. |
| static [MaxTokens](../../aspose.cells.ai/config/maxtokens/) | Максимальное количество токенов для ИИ за запрос |
| static [Temperature](../../aspose.cells.ai/config/temperature/) | Температура ИИ по умолчанию для использования. Когда температура приближается к 0, выбор модели становится очень детерминированным, почти всегда выбирая вывод с наивысшей вероятностью. Когда температура приближается к 1 или выше, вывод модели становится более случайным и разнообразным. |
| static [TimeOutSeconds](../../aspose.cells.ai/config/timeoutseconds/) | Время ожидания в секундах для ответа ИИ |

### См. также

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [CellsAI](../../)


