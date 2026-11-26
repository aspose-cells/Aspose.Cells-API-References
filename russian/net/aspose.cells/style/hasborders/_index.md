---
title: "Style.HasBorders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Проверяет, установлены ли границы для стиля"
type: docs
url: /ru/net/aspose.cells/style/hasborders/
---
## Style.HasBorders property

Проверяет, установлены ли границы для стиля.

```csharp
public bool HasBorders { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHasBordersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Получить доступ к ячейке A1 и проверить, есть ли у неё границы (по умолчанию должно быть false)
            Cell cellA1 = cells["A1"];
            Console.WriteLine("Cell A1 has borders: " + cellA1.GetStyle().HasBorders);

            // Создать стиль с границами
            Style styleWithBorders = workbook.CreateStyle();
            styleWithBorders.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            styleWithBorders.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Применить стиль к ячейке B1
            Cell cellB1 = cells["B1"];
            cellB1.SetStyle(styleWithBorders);

            // Проверить, есть ли у ячейки B1 границы (теперь должно быть true)
            Console.WriteLine("Cell B1 has borders: " + cellB1.GetStyle().HasBorders);

            // Сохраните книгу
            workbook.Save("HasBordersDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


