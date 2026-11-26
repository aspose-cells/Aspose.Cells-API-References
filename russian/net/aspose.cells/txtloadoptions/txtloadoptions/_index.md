---
title: "TxtLoadOptions.TxtLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор TxtLoadOptions. Создаёт параметры для загрузки текстового файла"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Создаёт параметры для загрузки текстового файла.

```csharp
public TxtLoadOptions()
```

### Примечания

Тип файла по умолчанию для загрузки — CSV.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создайте новый TxtLoadOptions с помощью конструктора
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            
            // Установите разделитель для CSV‑файла
            loadOptions.Separator = ',';
            
            // Создайте рабочую книгу с параметрами загрузки
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Выведите некоторую информацию из загруженного файла
            Console.WriteLine("Worksheet count: " + workbook.Worksheets.Count);
            Console.WriteLine("First cell value: " + workbook.Worksheets[0].Cells["A1"].Value);
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Создаёт параметры для загрузки текстового файла.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadFormat | LoadFormat | Формат загрузки |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class TxtLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Создайте примерное содержимое CSV и временный файл
            string csvData = "Column1,Column2,Column3\nData1,Data2,Data3";
            string tempFile = Path.GetTempFileName();
            File.WriteAllText(tempFile, csvData);

            try
            {
                // Создайте TxtLoadOptions с LoadFormat.Csv
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
                loadOptions.Separator = ',';
                loadOptions.HasTextQualifier = true;

                // Загрузите CSV, используя настроенные параметры
                Workbook workbook = new Workbook(tempFile, loadOptions);
                Worksheet worksheet = workbook.Worksheets[0];

                // Продемонстрируйте загруженные данные
                Console.WriteLine($"A1 Cell Value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 Cell Value: {worksheet.Cells["B2"].StringValue}");

                // Сохранить обработанную книгу
                workbook.Save("TxtLoadOptionsCtorDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor: {ex.Message}");
            }
            finally
            {
                // Очистить временный файл
                if (File.Exists(tempFile))
                {
                    File.Delete(tempFile);
                }
            }
        }
    }
}
```

### См. также

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


