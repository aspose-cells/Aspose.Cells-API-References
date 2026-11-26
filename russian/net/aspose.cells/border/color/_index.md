---
title: "Border.Color"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Border. Получает или задает цвет границы"
type: docs
url: /ru/net/aspose.cells/border/color/
---
## Border.Color property

Получает или задаёт цвет границы.

```csharp
public Color Color { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderPropertyColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Обратиться к ячейке A1
            Cell cell = worksheet.Cells["A1"];
            
            // Установить значение ячейки
            cell.PutValue("Border Color Demo");
            
            // Получить стиль ячейки
            Style style = cell.GetStyle();
            
            // Установить цвета и стили границы
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
            
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;
            
            style.Borders[BorderType.RightBorder].Color = Color.FromArgb(255, 128, 0); // Orange
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            
            // Применить стиль к ячейке
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("BorderColorDemo.xlsx");
            
            Console.WriteLine("Border color demo created successfully.");
        }
    }
}
```

### См. также

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


