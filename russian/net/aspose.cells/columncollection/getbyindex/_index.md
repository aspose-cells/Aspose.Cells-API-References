---
title: "ColumnCollection.GetByIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ColumnCollection. Возвращает объект столбца по индексу"
type: docs
url: /ru/net/aspose.cells/columncollection/getbyindex/
---
## ColumnCollection.GetByIndex method

Возвращает объект столбца по индексу.

```csharp
[Obsolete("Use Columns.GetColumnByIndex() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Column GetByIndex(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 |  |

### Возвращаемое значение

Возвращает объект столбца.

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте метод Columns.GetColumnByIndex(). Это свойство будет удалено через 12 месяцев, начиная с июня 2010 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте столбцы в коллекции, задав их ширины
            worksheet.Cells.Columns[0].Width = 15;  // Column 0
            worksheet.Cells.Columns[2].Width = 20;  // Column 2
            worksheet.Cells.Columns[4].Width = 25;  // Column 4

            try
            {
                // Получите второй столбец из ColumnCollection (индекс 1)
                Column column = worksheet.Cells.Columns.GetByIndex(1);

                Console.WriteLine($"Retrieved column at collection index 1");
                Console.WriteLine($"Worksheet column index: {column.Index}");
                Console.WriteLine($"Original width: {column.Width}");

                // Измените полученный столбец
                column.Width = 35;
                Console.WriteLine($"Updated width: {column.Width}");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ColumnCollectionGetByIndexDemo.xlsx");
        }
    }
}
```

### См. также

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


