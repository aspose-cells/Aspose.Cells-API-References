---
title: "BorderCollection.SetColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод BorderCollection. Устанавливает Color всех границ в коллекции"
type: docs
url: /ru/net/aspose.cells/bordercollection/setcolor/
---
## BorderCollection.SetColor method

Задает Color всех границ в коллекции.

```csharp
public void SetColor(Color color)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| цвет | Color | Color границ. |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderCollectionMethodSetColorWithColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль с цветными границами
            Style style = workbook.CreateStyle();
            
            // Установите стили линий границы
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Установите цвет границы в красный, используя метод SetColor
            style.Borders.SetColor(Color.Red);

            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with colored borders");
            cell.SetStyle(style);

            // Автоматически подгоните столбец для лучшей видимости
            worksheet.AutoFitColumn(0);

            // Сохраните книгу
            workbook.Save("BorderColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


