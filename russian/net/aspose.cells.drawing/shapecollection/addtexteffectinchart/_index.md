---
title: "ShapeCollection.AddTextEffectInChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Вставляет объект WordArt в диаграмму"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addtexteffectinchart/
---
## ShapeCollection.AddTextEffectInChart method

Вставляет объект WordArt на диаграмму.

```csharp
public Shape AddTextEffectInChart(MsoPresetTextEffect effect, string text, string fontName, 
    int size, bool fontBold, bool fontItalic, int top, int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| эффект | MsoPresetTextEffect | Тип предустановленного текстового эффекта mso. |
| текст | String | Текст WordArt. |
| fontName | String | Имя шрифта. |
| размер | Int32 | Размер шрифта |
| fontBold | Boolean | Указывает, является ли шрифт полужирным. |
| fontItalic | Boolean | Указывает, является ли шрифт курсивом. |
| верх | Int32 | Представляет вертикальное смещение фигуры от верхнего левого угла в единицах 1/4000 области диаграммы. |
| влево | Int32 | Представляет вертикальное смещение фигуры от верхнего левого угла в единицах 1/4000 области диаграммы. |
| высота | Int32 | Представляет высоту фигуры в единицах 1/4000 области диаграммы. |
| ширина | Int32 | Представляет ширину фигуры в единицах 1/4000 области диаграммы. |

### Возвращаемое значение

Возвращает объект Shape, представляющий новый объект WordArt.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectInChartWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            
            // Добавить WordArt на диаграмму
            Shape wordart = chart.Shapes.AddTextEffectInChart(
                MsoPresetTextEffect.TextEffect2,
                "SAMPLE TEXT", 
                "Arial Black", 
                36, 
                false, 
                false,
                100,  // Left position
                100,  // Top position
                300,  // Width
                200); // Height
                
            // Настроить внешний вид WordArt
            wordart.FillFormat.Transparency = 0.7;
            wordart.LineFormat.IsVisible = false;
            
            // Сохраните книгу
            workbook.Save("WordArtInChart.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


