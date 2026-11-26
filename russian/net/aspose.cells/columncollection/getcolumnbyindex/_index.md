---
title: "ColumnCollection.GetColumnByIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ColumnCollection. Возвращает объект Column по позиции в списке"
type: docs
url: /ru/net/aspose.cells/columncollection/getcolumnbyindex/
---
## ColumnCollection.GetColumnByIndex method

Возвращает объект [`Column`](../../column/) по позиции в списке.

```csharp
public Column GetColumnByIndex(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Позиция в списке. |

### Возвращаемое значение

Возвращает объект столбца.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetColumnByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные в столбец A
            worksheet.Cells["A1"].Value = "Aspose.Cells Column Demo";

            try
            {
                // Получите ссылку на коллекцию столбцов
                ColumnCollection columns = worksheet.Cells.Columns;

                // Получите доступ к столбцу с индексом 0 (столбец A) с помощью GetColumnByIndex
                Column column = columns.GetColumnByIndex(0);

                // Измените ширину столбца, чтобы продемонстрировать доступ к столбцу
                column.Width = 25;

                Console.WriteLine("Modified width of column at index 0 (Column A) to 25 characters.");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid column index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("ColumnCollectionMethodGetColumnByIndexWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


