---
title: "LowCodeSaveOptionsProviderOfAssembling.PathHeader"
second_title: "Справочник API Aspose.Cells для .NET"
description: "LowCodeSaveOptionsProviderOfAssembling свойство. Заголовочная часть перед добавленным содержимым листа и разделённой частью пути к файлу"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/
---
## LowCodeSaveOptionsProviderOfAssembling.PathHeader property

Часть заголовка (до добавленного содержимого листа и части разделения) пути файла.

```csharp
public string PathHeader { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathHeaderDemo
    {
        public static void Run()
        {
            // Создайте книгу с данными, которые будут разделены на несколько частей
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 150; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Инициализируйте провайдер параметров сохранения со значениями по умолчанию
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/QuarterlyReport_",
                PathTail = ".html",
                UseSheetName = true,
                SaveOptionsTemplate = new LowCodeSaveOptions() // Changed from HtmlSaveOptions to LowCodeSaveOptions
            };

            Console.WriteLine($"Initial PathHeader: {provider.PathHeader}");

            // Измените конфигурацию пути
            provider.PathHeader = "output/ModifiedReport_";
            provider.SheetPrefix = "Sheet_";
            provider.SplitPartPrefix = "Part_";

            // Продемонстрируйте эффект, сохранив с текущей конфигурацией провайдера
            workbook.Save("result.html", SaveFormat.Html); // Changed second parameter to SaveFormat.Html

            Console.WriteLine("Check 'output' directory for split files named like 'ModifiedReport_Sheet_0_Part_0.html'");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


