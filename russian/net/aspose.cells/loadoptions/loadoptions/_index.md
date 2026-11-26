---
title: "LoadOptions.LoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор LoadOptions. Создаёт параметры загрузки файла"
type: docs
url: /ru/net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Создаёт параметры загрузки файла.

```csharp
public LoadOptions()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";

            try
            {
                // Создайте пример содержимого CSV
                File.WriteAllText(tempCsvPath, "Name,Age\nJohn,30\nJane,25");

                // Продемонстрировать конструктор по умолчанию
                LoadOptions defaultOptions = new LoadOptions();
                Console.WriteLine("Default LoadFormat: " + defaultOptions.LoadFormat);

                // Продемонстрировать конструктор с параметром LoadFormat
                LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
                Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

                // Загрузить CSV‑файл с указанными параметрами
                Workbook workbook = new Workbook(tempCsvPath, csvOptions);

                // Проверьте, что данные были загружены корректно
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"Cell A1: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"Cell B2: {worksheet.Cells["B2"].StringValue}");

                // Сохранить как XLSX для демонстрации конверсии
                workbook.Save("CsvToExcel.xlsx");
                Console.WriteLine("CSV file successfully loaded and converted to XLSX");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

Создаёт параметры загрузки файла.

```csharp
public LoadOptions(LoadFormat loadFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadFormat | LoadFormat | Формат загрузки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";
            
            try
            {
                // Создайте пример содержимого CSV
                File.WriteAllText(tempCsvPath, "Column1,Column2\nData1,Data2");

                // Создать LoadOptions с LoadFormat.Csv
                LoadOptions options = new LoadOptions(LoadFormat.Csv);

                // Загрузить CSV‑файл с созданными параметрами
                Workbook workbook = new Workbook(tempCsvPath, options);

                // Продемонстрировать успешную загрузку, чтением ячейки
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"A1 cell value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 cell value: {worksheet.Cells["B2"].StringValue}");

                // Сохранить как XLSX для демонстрации возможности конверсии
                workbook.Save("CsvLoadedAsExcel.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during CSV loading: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### См. также

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


