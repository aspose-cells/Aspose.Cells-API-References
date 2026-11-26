---
title: "Style.Borders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает BorderCollection стиля"
type: docs
url: /ru/net/aspose.cells/style/borders/
---
## Style.Borders property

Получает [`BorderCollection`](../../bordercollection/) стиля.

```csharp
public BorderCollection Borders { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBordersDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить ячейку и её стиль
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            
            // Установить разные стили границ
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Medium;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            
            // Применить стиль к ячейке
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("BorderStylesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [BorderCollection](../../bordercollection/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


