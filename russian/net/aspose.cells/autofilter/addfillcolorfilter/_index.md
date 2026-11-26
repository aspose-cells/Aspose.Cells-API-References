---
title: "AutoFilter.AddFillColorFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Добавляет фильтр по цвету заливки"
type: docs
url: /ru/net/aspose.cells/autofilter/addfillcolorfilter/
---
## AutoFilter.AddFillColorFilter method

Добавляет фильтр по цвету заливки.

```csharp
public void AddFillColorFilter(int fieldIndex, BackgroundType pattern, CellsColor foregroundColor, 
    CellsColor backgroundColor)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| шаблон | BackgroundType | Тип шаблона фона. |
| foregroundColor | CellsColor | Цвет переднего плана. |
| backgroundColor | CellsColor | Цвет фона. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFillColorFilterWithInt32BackgroundTypeCellsColorCDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные с разными цветами заливки
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");
            
            // Применить разные цвета заливки
            Style style1 = cells["A2"].GetStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style1);
            
            Style style2 = cells["A3"].GetStyle();
            style2.ForegroundColor = Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style2);
            
            Style style3 = cells["A4"].GetStyle();
            style3.ForegroundColor = Color.Green;
            style3.Pattern = BackgroundType.Solid;
            cells["A4"].SetStyle(style3);

            // Создать автофильтр
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Создать цвет ячеек для фильтрации
            CellsColor filterColor = workbook.CreateCellsColor();
            filterColor.Color = Color.Red;
            
            // Применить фильтр по цвету заливки
            filter.AddFillColorFilter(0, BackgroundType.Solid, filterColor, filterColor);
            filter.Refresh();
            
            // Сохраните книгу
            workbook.Save("AutoFilterFillColorDemo.xlsx");
        }
    }
}
```

### См. также

* enum [BackgroundType](../../backgroundtype/)
* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


