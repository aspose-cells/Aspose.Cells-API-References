---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptionsProviderOfPlaceHolders. Префикс для индекса части разделения"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix property

Префикс для индекса части разделения.

```csharp
public string SplitPartPrefix { get; set; }
```

### Примечания

Если существует только одна часть разделения и [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) равно false, то этот префикс и индекс части разделения (0) не будут добавлены в результирующий путь к файлу.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Настроить шаблон параметров сохранения
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();

            // Инициализируйте провайдер с заполнительным параметром части разделения
            LowCodeSaveOptionsProviderOfPlaceHolders provider = new LowCodeSaveOptionsProviderOfPlaceHolders("SplitResult_Sheet{sheet}_Part{split}.xlsx")
            {
                SaveOptionsTemplate = saveOptionsTemplate
            };

            // Отобразите и измените SplitPartPrefix
            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");
            provider.SplitPartPrefix = "Section";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Сохраните книгу с разделёнными частями, используя формат сохранения провайдера
            workbook.Save("output", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'output' directory for split files with 'Section' prefix");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


