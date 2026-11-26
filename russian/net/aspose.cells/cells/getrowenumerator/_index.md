---
title: "Cells.GetRowEnumerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает перечислитель строк."
type: docs
url: /ru/net/aspose.cells/cells/getrowenumerator/
---
## Cells.GetRowEnumerator method

Получает перечислитель строк.

```csharp
[Obsolete("Use RowCollection.GetEnumerator() method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetRowEnumerator()
```

### Возвращаемое значение

Перечислитель строк.

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод RowCollection.GetEnumerator(). Этот метод будет удалён через 12 месяцев, начиная с мая 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetRowEnumeratorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Row 1 Data");
            worksheet.Cells["A3"].PutValue("Row 3 Data");
            worksheet.Cells["A5"].PutValue("Row 5 Data");

            try
            {
                // Получите перечислитель строк из коллекции Cells.
                IEnumerator enumerator = worksheet.Cells.GetRowEnumerator();
                
                Console.WriteLine("Iterating through rows containing data:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Cell cell = row.GetCellOrNull(0); // Get first cell in row
                    string cellValue = cell != null ? cell.Value.ToString() : "empty";
                    Console.WriteLine($"Row {row.Index}: First cell value = {cellValue}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowEnumerator method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("MethodGetRowEnumeratorDemo.xlsx");
        }
    }
}
```

### См. также

* method [GetEnumerator](../../rowcollection/getenumerator/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


