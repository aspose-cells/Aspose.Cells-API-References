---
title: "ColorFilter.GetColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ColorFilter. Получает цвет этого фильтра"
type: docs
url: /ru/net/aspose.cells/colorfilter/getcolor/
---
## ColorFilter.GetColor method

Получает цвет этого фильтра.

```csharp
public Color GetColor(WorksheetCollection sheets)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| листы | WorksheetCollection |  |

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterMethodGetColorWithWorksheetCollectionDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");
            
            // Создать автофильтр
            worksheet.AutoFilter.Range = "A1:A4";
            
            // Создать цветовой фильтр
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            worksheet.AutoFilter.Refresh();
            
            // Получить фильтр цвета и проверить его цвет
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            if (colorFilter != null)
            {
                Color retrievedColor = colorFilter.GetColor(workbook.Worksheets);
                Console.WriteLine("Filter color: " + retrievedColor.ToString());
            }
        }
    }
}
```

### См. также

* class [WorksheetCollection](../../worksheetcollection/)
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


