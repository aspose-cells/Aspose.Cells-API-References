---
title: "Класс SplitPartInfo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LowCode.SplitPartInfo. Представляет информацию об одном вводе/выводе для множественных вводов/выводов, например текущей странице, которая будет отрисована при конвертации таблицы в изображение"
type: docs
url: /ru/net/aspose.cells.lowcode/splitpartinfo/
---
## SplitPartInfo class

Представляет информацию одного входа/выхода для нескольких входов/выходов, например текущей страницы, которая будет отрисована при преобразовании электронной таблицы в изображение.

```csharp
public class SplitPartInfo
```

## Свойства

| Имя | Описание |
| --- | --- |
| [PartIndex](../../aspose.cells.lowcode/splitpartinfo/partindex/) { get; } | Индекс текущей части в последовательности (нумерация с нуля). -1 означает отсутствие нескольких частей, поэтому результат один. |
| [SheetIndex](../../aspose.cells.lowcode/splitpartinfo/sheetindex/) { get; } | Индекс листа, в котором находится текущая часть. -1 обозначает, что лист только один. |
| [SheetName](../../aspose.cells.lowcode/splitpartinfo/sheetname/) { get; } | Имя листа, в котором находится текущая часть. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте книгу с несколькими листами для демонстрации
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Создать LowCodeLoadOptions и LowCodeSplitOptions
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;

                // Создать пользовательского провайдера для демонстрации использования SplitPartInfo
                splitOptions.SaveOptionsProvider = new CustomSplitOptionsProvider();

                // Выполнить операцию разбиения
                SpreadsheetSplitter.Process(splitOptions);

                Console.WriteLine("Split operation completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSplitOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Продемонстрировать доступ к свойствам SplitPartInfo
            Console.WriteLine($"Processing part: Index={partInfo.PartIndex}, SheetIndex={partInfo.SheetIndex}, SheetName={partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


