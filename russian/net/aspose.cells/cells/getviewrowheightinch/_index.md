---
title: "Cells.GetViewRowHeightInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает высоту указанной строки в единицах дюймов"
type: docs
url: /ru/net/aspose.cells/cells/getviewrowheightinch/
---
## Cells.GetViewRowHeightInch method

Получает высоту указанной строки в дюймах.

```csharp
public double GetViewRowHeightInch(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки |

### Возвращаемое значение

Высота строки

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetViewRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите пользовательскую высоту строки для строки 2 в дюймах
            worksheet.Cells.SetRowHeightInch(2, 1.5);

            try
            {
                // Вызовите GetViewRowHeightInch с параметром индекса строки
                double rowHeight = worksheet.Cells.GetViewRowHeightInch(2);
                
                // Отобразите результат и проверьте, что высота соответствует установленному значению
                Console.WriteLine($"View row height of row 2: {rowHeight} inches");
                
                // Продемонстрируйте эффект, добавив примерное содержимое
                worksheet.Cells["A2"].PutValue($"Row Height: {rowHeight}\"");
                worksheet.Cells.SetColumnWidthInch(0, 15);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetViewRowHeightInch: {ex.Message}");
            }
            
            // Сохранить изменённую книгу
            workbook.Save("CellsMethodGetViewRowHeightInchWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


