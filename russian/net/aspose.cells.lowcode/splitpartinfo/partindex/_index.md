---
title: "SplitPartInfo.PartIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SplitPartInfo. Индекс текущей части в последовательности, начиная с 0. 1 означает, что нет нескольких частей, поэтому результат один."
type: docs
url: /ru/net/aspose.cells.lowcode/splitpartinfo/partindex/
---
## SplitPartInfo.PartIndex property

Индекс текущей части в последовательности (нумерация с нуля). -1 означает отсутствие нескольких частей, поэтому результат один.

```csharp
public int PartIndex { get; }
```

### Примечания

Если необходимо обработать несколько листов и каждый лист обрабатывается (разделяется) отдельно, индекс части всегда начинается с 0 для каждого листа. Например, при конвертации книги в изображения он представляет индекс выходной страницы текущего обрабатываемого листа. А значение -1 обозначает, что для текущего листа существует только одна страница.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Создать книгу с несколькими листами
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Сохранить книгу для использования в операции разделения
                workbook.Save("sample.xlsx");

                // Создать параметры загрузки
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                // Создать параметры разделения с пользовательским провайдером
                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;
                splitOptions.SaveOptionsProvider = new CustomPartIndexProvider();

                // Выполнить операцию разбиения
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomPartIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Продемонстрировать чтение свойства PartIndex
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### См. также

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


