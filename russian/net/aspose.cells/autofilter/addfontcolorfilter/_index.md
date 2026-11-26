---
title: "AutoFilter.AddFontColorFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Добавляет фильтр по цвету шрифта"
type: docs
url: /ru/net/aspose.cells/autofilter/addfontcolorfilter/
---
## AutoFilter.AddFontColorFilter method

Добавляет фильтр по цвету шрифта.

```csharp
public void AddFontColorFilter(int fieldIndex, CellsColor color)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| color | CellsColor | Объект [`CellsColor`](../../cellscolor/). |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFontColorFilterWithInt32CellsColorDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные с разными цветами шрифта
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Item 1");
            cells["A3"].PutValue("Item 2");
            cells["A4"].PutValue("Item 3");
            
            // Установите цвета шрифта
            Style style = cells["A2"].GetStyle();
            style.Font.Color = Color.Red;
            cells["A2"].SetStyle(style);
            
            style = cells["A3"].GetStyle();
            style.Font.Color = Color.Blue;
            cells["A3"].SetStyle(style);
            
            style = cells["A4"].GetStyle();
            style.Font.Color = Color.Green;
            cells["A4"].SetStyle(style);

            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Создайте цветовой фильтр для красного шрифта
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            
            // Добавьте фильтр по цвету шрифта
            filter.AddFontColorFilter(0, cr);
            filter.Refresh();
            
            // Сохраните книгу
            workbook.Save("AutoFilterFontColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


