---
title: "Cells.GetRowOriginalHeightPoint"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает оригинальную высоту строки в пунктах, если строка скрыта"
type: docs
url: /ru/net/aspose.cells/cells/getroworiginalheightpoint/
---
## Cells.GetRowOriginalHeightPoint method

Получает оригинальную высоту строки в пунктах, если строка скрыта

```csharp
[Obsolete("Use Cells.GetRowHeight(int,bool,CellsUnitType) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetRowOriginalHeightPoint(int row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Cells.GetRowHeight(int,bool,CellsUnitType). Этот метод будет удалён через 12 месяцев, начиная с апреля 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowOriginalHeightPointWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Сохранить оригинальную высоту перед изменением
            double originalHeightBefore = cells.GetRowOriginalHeightPoint(0);
            
            // Изменить высоту строки
            cells.SetRowHeight(0, 25.5);

            try
            {
                // Получить оригинальную высоту после изменения
                double originalHeight = cells.GetRowOriginalHeightPoint(0);
                double currentHeight = cells.GetRowHeight(0);

                Console.WriteLine($"Original row height: {originalHeight} points");
                Console.WriteLine($"Current row height: {currentHeight} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowOriginalHeightPoint: {ex.Message}");
            }

            workbook.Save("GetRowOriginalHeightPointDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


