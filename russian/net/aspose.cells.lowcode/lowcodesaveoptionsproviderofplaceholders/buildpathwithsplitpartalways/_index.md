---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptionsProviderOfPlaceHolders. Добавлять ли индекс части разбиения в путь к файлу всегда. Значение по умолчанию — false, то есть когда существует только одна часть разбиения, индекс части разбиения и соответствующий префикс prefixSplitPartPrefix не будут добавлены в путь к файлу"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways property

Добавлять ли индекс части разбиения в путь к файлу всегда. Значение по умолчанию — false, то есть когда существует только одна часть разбиения, индекс части разбиения и соответствующий префикс([`SplitPartPrefix`](../splitpartprefix/)) не будут добавлены в путь к файлу.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSplitPartAlwaysDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с данными, которые не будут разбиты на несколько частей
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Single Part Demonstration";

            // Создать провайдер с шаблоном пути и условием разбиения, которое приводит к одной части
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Result_{split}.xlsx")
            {
                SaveOptionsTemplate = new LowCodeSaveOptions()
            };

            // Продемонстрировать состояние свойства false (по умолчанию)
            Console.WriteLine($"Initial BuildPathWithSplitPartAlways: {provider.BuildPathWithSplitPartAlways}");
            provider.BuildPathWithSplitPartAlways = false;
            
            // Это сгенерирует файл Result.xlsx, когда существует только одна часть
            Console.WriteLine("Saving with BuildPathWithSplitPartAlways=false");
            ExecuteDummySave(workbook, "Result.xlsx");

            // Переключить свойство и продемонстрировать состояние true
            provider.BuildPathWithSplitPartAlways = true;
            Console.WriteLine("\nSaving with BuildPathWithSplitPartAlways=true");
            
            // Это сгенерирует файл Result_0.xlsx даже при одной части
            ExecuteDummySave(workbook, "Result_0.xlsx");
        }

        private static void ExecuteDummySave(Workbook workbook, string filename)
        {
            // В реальном использовании замените на операцию сохранения на основе провайдера
            Console.WriteLine($"Simulated save operation -> Filename: {filename}");
            workbook.Save(filename, SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


