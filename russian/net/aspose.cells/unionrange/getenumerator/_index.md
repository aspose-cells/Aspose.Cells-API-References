---
title: "UnionRange.GetEnumerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод UnionRange. Возвращает перечислитель для ячеек в этом диапазоне"
type: docs
url: /ru/net/aspose.cells/unionrange/getenumerator/
---
## UnionRange.GetEnumerator method

Получает перечислитель для ячеек в этом Range.

```csharp
public IEnumerator GetEnumerator()
```

### Возвращаемое значение

Перечислитель ячеек

### Примечания

При обходе элементов с помощью возвращённого Enumerator, коллекцию Cells не следует изменять(например, операции, которые приведут к созданию новых Cell/Row или удалению существующих Cell/Row). В противном случае перечислитель может не суметь корректно пройти все ячейки(некоторые элементы могут быть пройдены несколько раз или пропущены).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class UnionRangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте первый диапазон (A1:B2) и заполните его данными
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1", "B2");
            range1[0, 0].PutValue("R1C1");
            range1[0, 1].PutValue("R1C2");
            range1[1, 0].PutValue("R2C1");
            range1[1, 1].PutValue("R2C2");

            // Создайте второй диапазон (C1:D2) и заполните его данными
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("C1", "D2");
            range2[0, 0].PutValue("R1C3");
            range2[0, 1].PutValue("R1C4");
            range2[1, 0].PutValue("R2C3");
            range2[1, 1].PutValue("R2C4");

            try
            {
                // Создайте UnionRange из первого диапазона
                UnionRange unionRange = worksheet.Cells
                    .CreateRange("A1:B2")
                    .UnionRanges(new Aspose.Cells.Range[] { range1 });

                // Добавьте второй диапазон к объединению
                unionRange = unionRange.Union("C1:D2");

                // Получите перечислитель и пройдитесь по всем ячейкам в объединении
                IEnumerator enumerator = unionRange.GetEnumerator();
                Console.WriteLine("Enumerating cells in the UnionRange:");
                while (enumerator.MoveNext())
                {
                    Cell cell = enumerator.Current as Cell;
                    if (cell != null)
                    {
                        Console.WriteLine($"{cell.Name}: {cell.Value}");
                    }
                }

                // Сохраните книгу (необязательно, только чтобы показать, что данные сохраняются)
                workbook.Save("UnionRangeGetEnumeratorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetEnumerator: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


