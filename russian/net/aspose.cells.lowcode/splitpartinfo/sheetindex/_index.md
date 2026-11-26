---
title: "SplitPartInfo.SheetIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SplitPartInfo. Индекс листа, в котором находится текущая часть. 1 обозначает, что лист только один."
type: docs
url: /ru/net/aspose.cells.lowcode/splitpartinfo/sheetindex/
---
## SplitPartInfo.SheetIndex property

Индекс листа, в котором находится текущая часть. -1 обозначает, что лист только один.

```csharp
public int SheetIndex { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertySheetIndexDemo
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
                splitOptions.SaveOptionsProvider = new CustomSheetIndexProvider();

                // Выполнить операцию разбиения
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSheetIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Продемонстрировать чтение свойства SheetIndex
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Sheet_{partInfo.SheetIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### См. также

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


