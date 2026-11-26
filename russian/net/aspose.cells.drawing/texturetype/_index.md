---
title: "Перечисление TextureType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.TextureType. Представляет предустановленный тип текстуры"
type: docs
url: /ru/net/aspose.cells.drawing/texturetype/
---
## TextureType enumeration

Представляет тип предустановленной текстуры.

```csharp
public enum TextureType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| BlueTissuePaper | `0` | Представляет тип текстуры Blue Tissue Paper. |
| Bouquet | `1` | Представляет тип текстуры Bouquet. |
| BrownMarble | `2` | Представляет тип текстуры Brown Marble. |
| Canvas | `3` | Представляет тип текстуры Canvas. |
| Cork | `4` | Представляет тип текстуры Cork. |
| Denim | `5` | Представляет тип текстуры Denim. |
| FishFossil | `6` | Представляет тип текстуры Fish Fossil. |
| Granite | `7` | Представляет тип текстуры Granite. |
| GreenMarble | `8` | Представляет тип текстуры Green Marble. |
| MediumWood | `9` | Представляет тип текстуры Medium Wood. |
| Newsprint | `10` | Представляет тип текстуры Newsprint. |
| Oak | `11` | Представляет тип текстуры Oak. |
| PaperBag | `12` | Представляет тип текстуры Paper Bag. |
| Papyrus | `13` | Представляет тип текстуры Papyrus. |
| Parchment | `14` | Представляет тип текстуры Parchment. |
| PinkTissuePaper | `15` | Представляет тип текстуры Pink Tissue Paper. |
| PurpleMesh | `16` | Представляет тип текстуры Purple Mesh. |
| RecycledPaper | `17` | Представляет тип текстуры Recycled Paper. |
| Sand | `18` | Представляет тип текстуры Sand. |
| Stationery | `19` | Представляет тип текстуры Stationery. |
| Walnut | `20` | Представляет тип текстуры Walnut Droplets. |
| WaterDroplets | `21` | Представляет тип текстуры Water Droplets. |
| WhiteMarble | `22` | Представляет тип текстуры White Marble. |
| WovenMat | `23` | Представляет тип текстуры Woven Mat. |
| Unknown | `24` | Представляет тип текстуры Unknown. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextureTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите доступ к первой серии и задайте текстуру для точки
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Stationery;

            // Сохраните книгу
            workbook.Save("TextureTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


