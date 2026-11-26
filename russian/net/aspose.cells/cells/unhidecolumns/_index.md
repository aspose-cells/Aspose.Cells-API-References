---
title: "Cells.UnhideColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Отображает несколько скрытых столбцов"
type: docs
url: /ru/net/aspose.cells/cells/unhidecolumns/
---
## Cells.UnhideColumns method

Отображает несколько скрытых столбцов.

```csharp
public void UnhideColumns(int column, int totalColumns, double width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |
| totalColumns | Int32 | Номер столбца |
| ширина | Double | Ширина столбца. |

### Примечания

Применяется только к ширине скрытых столбцов.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUnhideColumnsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            // Создать новую книгу и получить доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Сначала скрыть столбцы 1-3 (нумерация с нуля)
            worksheet.Cells.HideColumns(1, 3);

            try
            {
                // Отобразить столбцы, начиная с индекса 1 (второй столбец), шириной 3 столбца, установить ширину 15,5
                worksheet.Cells.UnhideColumns(1, 3, 15.5);

                // Проверьте отображённые столбцы, проверив их ширину
                Console.WriteLine($"Column 1 width after unhiding: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine("Columns 1-3 successfully unhidden with specified width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnhideColumns: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("UnhideColumnsWithWidthDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


