---
title: "Range.ClearContents"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Очищает содержимое этого диапазона"
type: docs
url: /ru/net/aspose.cells/range/clearcontents/
---
## Range.ClearContents method

Очищает содержимое этого диапазона.

```csharp
public void ClearContents()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearContentsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые примерные данные, чтобы продемонстрировать очистку
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue("Sample");
            worksheet.Cells["B2"].PutValue("Data");

            try
            {
                // Создайте диапазон, охватывающий ячейки A1:B2
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Отобразите содержимое диапазона до очистки
                Console.WriteLine("Before clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Вызовите ClearContents, чтобы удалить все значения в диапазоне
                range.ClearContents();

                // Отобразите содержимое диапазона после очистки
                Console.WriteLine("\nAfter clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Сохраните книгу
                workbook.Save("ClearContentsDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


