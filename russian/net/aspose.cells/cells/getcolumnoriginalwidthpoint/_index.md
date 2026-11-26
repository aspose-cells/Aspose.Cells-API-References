---
title: "Cells.GetColumnOriginalWidthPoint"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает исходную высоту столбца в единицах точек, если столбец скрыт"
type: docs
url: /ru/net/aspose.cells/cells/getcolumnoriginalwidthpoint/
---
## Cells.GetColumnOriginalWidthPoint method

Получает исходную высоту столбца в единицах точек, если столбец скрыт

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnOriginalWidthPoint(int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс строки. |

### Возвращаемое значение

Ширина столбца в обычном виде.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Cells.GetColumnWidth(int ,bool , CellsUnitType ). Этот метод будет удалён через 12 месяцев, начиная с апреля 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnOriginalWidthPointWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Подготовьте параметр индекса столбца
            int columnIndex = 0;

            try
            {
                // Получить исходную ширину столбца в точках
                double originalWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width of column {columnIndex}: {originalWidth} points");

                // Изменить ширину столбца
                cells.SetColumnWidth(columnIndex, 15);
                Console.WriteLine("Set new column width to 15 points");

                // Снова получить исходную ширину, чтобы продемонстрировать, что она осталась неизменной
                double unchangedWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width remains: {unchangedWidth} points");

                // Получить текущую ширину, чтобы показать изменение
                double currentWidth = cells.GetColumnWidth(columnIndex);
                Console.WriteLine($"Current column width: {currentWidth} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnOriginalWidthPoint method: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("GetColumnOriginalWidthPointDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


