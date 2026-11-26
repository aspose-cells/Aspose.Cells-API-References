---
title: "SpreadsheetSplitter.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SpreadsheetSplitter. Делит указанный файл шаблона на несколько частей"
type: docs
url: /ru/net/aspose.cells.lowcode/spreadsheetsplitter/process/
---
## Process(string, string) {#process_1}

Разделяет указанный файл шаблона на несколько частей.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| templateFile | String | Файл шаблона, который нужно разделить |
| resultFile | String | Результирующий файл (шаблон имени) |

### Примечания

Файлы вывода будут создаваться из указанного результирующего файла путем добавления порядкового номера листа и части. Например, если указанный файл вывода — Split.xlsx, то сгенерированные файлы будут Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetSplitterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу с несколькими листами
            Workbook templateWorkbook = new Workbook();
            Worksheet sheet1 = templateWorkbook.Worksheets.Add("SalesData");
            sheet1.Cells["A1"].PutValue("Product");
            Worksheet sheet2 = templateWorkbook.Worksheets.Add("Inventory");
            sheet2.Cells["A1"].PutValue("test data");

            // Сохранить как файл шаблона
            string templatePath = "SplitterTemplate.xlsx";
            templateWorkbook.Save(templatePath, SaveFormat.Xlsx);

            // Определите шаблон вывода результата
            string resultPattern = "SplitResult_";
            
            try
            {
                // Обработайте шаблон напрямую, используя статический метод
                SpreadsheetSplitter.Process(templatePath, resultPattern);
                
                Console.WriteLine($"Spreadsheet split successfully using pattern: {resultPattern}");
                Console.WriteLine("Check output directory for split files");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during spreadsheet splitting: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeSplitOptions) {#process}

Разделяет файл электронной таблицы на несколько частей.

```csharp
public static void Process(LowCodeSplitOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | LowCodeSplitOptions | Параметры для разделения электронной таблицы |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetSplitterMethodProcessWithLowCodeSplitOptionsDemo
    {
        public static void Run()
        {

            // Инициализировать параметры разделения
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions
            {
                LoadOptions = new LowCodeLoadOptions { InputFile = "split.xlsx" },
                SaveOptionsProvider = new CustomLowCodeSaveOptionsProvider()
            };

            try
            {
                // Выполнить разделение таблицы с использованием статического метода
                SpreadsheetSplitter.Process(splitOptions);
                
                Console.WriteLine($"Spreadsheet split successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Split operation failed: {ex.Message}");
            }
        }
    }

    // Конкретная реализация AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        {
            base.Finish(part);
        }
        // Реализуйте требуемый абстрактный метод
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### См. также

* class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


