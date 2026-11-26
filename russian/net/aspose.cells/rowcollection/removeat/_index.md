---
title: "RowCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод RowCollection. Удаляет элемент строки в указанной позиции индекса в этой коллекции"
type: docs
url: /ru/net/aspose.cells/rowcollection/removeat/
---
## RowCollection.RemoveAt method

Удаляет элемент строки по указанному индексу (позиции) в этой коллекции.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| index | Int32 | Нулевой индекс (позиция, а не [`Index`](../../row/index/)) существующего элемента строки в этой коллекции. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные в ячейки первых нескольких строк
            worksheet.Cells["A1"].PutValue("Row 1");
            worksheet.Cells["A2"].PutValue("Row 2");
            worksheet.Cells["A3"].PutValue("Row 3");
            worksheet.Cells["A4"].PutValue("Row 4");

            // Отобразите начальное количество строк
            Console.WriteLine($"Initial row count: {worksheet.Cells.Rows.Count}");

            try
            {
                // Вызовите метод RemoveAt, чтобы удалить строку с индексом 1 (вторая строка)
                worksheet.Cells.Rows.RemoveAt(1);

                Console.WriteLine("Method executed successfully. Row at index 1 removed.");

                // Отобразите обновлённое количество строк
                Console.WriteLine($"Updated row count: {worksheet.Cells.Rows.Count}");

                // Покажите эффект — строка 2 должна быть удалена, строка 3 становится строкой 2
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("RowCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


