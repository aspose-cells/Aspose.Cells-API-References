---
title: "Cells.GetColumnWidthInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает ширину указанного столбца в обычном виде в дюймах"
type: docs
url: /ru/net/aspose.cells/cells/getcolumnwidthinch/
---
## Cells.GetColumnWidthInch method

Получает ширину указанного столбца в обычном виде, в дюймах.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnWidthInch(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца |

### Возвращаемое значение

Ширина столбца

Ширина столбца в обычном виде.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Cells.GetColumnWidth(int ,bool , CellsUnitType ). Этот метод будет удалён через 12 месяцев, начиная с апреля 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthInchWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить ширину столбца в дюймах для демонстрации
            int columnIndex = 2;
            cells.SetColumnWidthInch(columnIndex, 2.5);

            try
            {
                // Вызвать GetColumnWidthInch с параметром типа Int32
                double columnWidth = cells.GetColumnWidthInch(columnIndex);

                // Отобразить результат
                Console.WriteLine($"Width of column {columnIndex} in inches: {columnWidth}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthInch method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("CellsMethodGetColumnWidthInchDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


