---
title: "UnionRange.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnionRange. Копирование диапазона с параметрами специальной вставки"
type: docs
url: /ru/net/aspose.cells/unionrange/copy/
---
## UnionRange.Copy method

Копирует диапазон с параметрами специальной вставки.

```csharp
public void Copy(UnionRange range, PasteOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| диапазон | UnionRange | Исходный диапазон. |
| опции | PasteOptions | Параметры специальной вставки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodCopyWithUnionRangePasteOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Value2");

            try
            {
                // Создайте исходный UnionRange
                UnionRange sourceRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // Создайте целевой UnionRange
                UnionRange destinationRange = worksheet.Cells.CreateRange("D1:E2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("D1:E2") });

                // Создайте PasteOptions с конкретными настройками
                PasteOptions options = new PasteOptions();
                options.PasteType = PasteType.All;
                options.SkipBlanks = true;
                options.Transpose = false;

                // Вызовите метод Copy
                sourceRange.Copy(destinationRange, options);

                Console.WriteLine("Copy method executed successfully");
                Console.WriteLine($"Destination range: {destinationRange.RefersTo}");

                // Сохраните книгу
                workbook.Save("UnionRangeCopyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Copy: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PasteOptions](../../pasteoptions/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


