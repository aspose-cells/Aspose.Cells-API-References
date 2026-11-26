---
title: "SpreadsheetMerger.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SpreadsheetMerger. Объединить указанные файлы шаблонов"
type: docs
url: /ru/net/aspose.cells.lowcode/spreadsheetmerger/process/
---
## Process(string[], string) {#process_1}

Объединить указанные файлы шаблонов.

```csharp
public static void Process(string[] templateFiles, string resultFile)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| templateFiles | String[] | Файлы шаблонов для объединения |
| resultFile | String | Полученный файл |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithStringArrayStringDemo
    {
        public static void Run()
        {
            // Создать примерные файлы шаблонов
            CreateTemplateFile("template1.xlsx", "Data from Template 1");
            CreateTemplateFile("template2.xlsx", "Data from Template 2");

            string[] templateFiles = { "template1.xlsx", "template2.xlsx" };
            string resultFile = "merged_output.xlsx";

            try
            {
                SpreadsheetMerger.Process(templateFiles, resultFile);

                Console.WriteLine($"Process method merged {templateFiles.Length} files into {resultFile}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### См. также

* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeMergeOptions) {#process}

Объединяет несколько шаблонных файлов в один.

```csharp
public static void Process(LowCodeMergeOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | LowCodeMergeOptions | Параметры для объединения файлов |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithLowCodeMergeOptDemo
    {
        public static void Run()
        {
            // Подготовьте два простых файла шаблона, которые будут объединены.
            CreateTemplateFile("TemplateA.xlsx", "Data from Template A");
            CreateTemplateFile("TemplateB.xlsx", "Data from Template B");

            try
            {
                // Создать экземпляр класса параметров.
                // Класс LowCodeMergeOptions является частью Aspose.Cells.LowCode.
                // Для этой демонстрации мы используем конструктор по умолчанию.
                LowCodeMergeOptions options = new LowCodeMergeOptions();

                // Вызовите метод Process, который принимает LowCodeMergeOptions.
                SpreadsheetMerger.Process(options);

                Console.WriteLine("Process method invoked successfully with LowCodeMergeOptions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### См. также

* class [LowCodeMergeOptions](../../lowcodemergeoptions/)
* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


