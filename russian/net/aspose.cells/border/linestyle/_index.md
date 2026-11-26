---
title: "Border.LineStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Border. Получает или задает тип границы ячейки"
type: docs
url: /ru/net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

Получает или задаёт тип границы ячейки.

```csharp
public CellBorderType LineStyle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyLineStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратиться к ячейке и получить её стиль
            Cell cell = worksheet.Cells["B2"];
            Style style = cell.GetStyle();

            // Установить различные стили линий границы
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;

            // Применить стиль к ячейке
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("BorderLineStyleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


