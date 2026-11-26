---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptionsProviderOfPlaceHolders. Добавлять ли индекс листа или его имя в путь к файлу всегда. Значение по умолчанию — false, то есть когда существует только один лист, индекс листа и имя и соответствующий префикс prefixSheetNamePrefix не будут добавлены в путь к файлу"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways property

Добавлять ли индекс листа или его имя в путь к файлу всегда. Значение по умолчанию — false, то есть когда существует только один лист, индекс листа и имя и соответствующий префикс([`SheetNamePrefix`](../sheetnameprefix/)) не будут добавлены в путь к файлу.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с двумя листами, чтобы продемонстрировать различия в путях
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Настроить провайдер с заполнителем индекса листа
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_{sheet_index}.xlsx")
            {
                // Продемонстрировать смещение индекса листа (опционально)
                SheetIndexOffset = 1
            };

            Console.WriteLine($"Initial BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");

            // Сохранять с индексом листа только при наличии нескольких листов (поведение по умолчанию)
            provider.BuildPathWithSheetAlways = false;
            SaveWithProvider(workbook, provider, "DefaultBehavior");

            // Принудительно добавлять индекс листа в имена файлов даже для одиночных листов
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine($"Modified BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
            SaveWithProvider(workbook, provider, "ForcedSheetIndex");
        }

        private static void SaveWithProvider(Workbook workbook, LowCodeSaveOptionsProviderOfPlaceHolders provider, string saveDescription)
        {
            // Настроить параметры сохранения в формате JSON для включения разбиения
            var saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Json
            };

            // Настройте провайдер с параметрами сохранения
            provider.SaveOptionsTemplate = saveOptions;

            // Сохранить с путями, определяемыми провайдером
            Console.WriteLine($"Saving with {saveDescription} - check output files");
            workbook.Save($"dummy_{saveDescription}.json", saveOptions.SaveFormat);
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


