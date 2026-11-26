---
title: "ShapeCollection.AddShapeInChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет фигуру в диаграмму. Все единицы измерения — 1/4000 области диаграммы"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addshapeinchart/
---
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}

Добавить форму на диаграмму. Все единицы — 1/4000 области диаграммы.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom, byte[] imageData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | MsoDrawingType | Тип рисования. |
| размещение | PlacementType | тип размещения. |
| влево | Int32 | В единицах ширины области диаграммы 1/4000. |
| верх | Int32 | В единицах высоты области диаграммы 1/4000. |
| право | Int32 | В единицах ширины области диаграммы 1/4000. |
| низ | Int32 | В единицах высоты области диаграммы 1/4000. |
| imageData | Byte[] | Если фигура не является изображением или объектом OLE, imageData должно быть null. |

### См. также

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}

Добавить форму на диаграмму. Все единицы — 1/4000 области диаграммы.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | MsoDrawingType | Тип рисования. |
| размещение | PlacementType | тип размещения. |
| влево | Int32 | В единицах ширины области диаграммы 1/4000. |
| верх | Int32 | В единицах высоты области диаграммы 1/4000. |
| право | Int32 | В единицах ширины области диаграммы 1/4000. |
| низ | Int32 | В единицах высоты области диаграммы 1/4000. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartWithMsoDrawingTypePlacementTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Добавить фигуру в диаграмму
            chart.Shapes.AddShapeInChart(MsoDrawingType.CheckBox, PlacementType.Move, 100, 100, 1000, 1000);
            
            // Установить текст фигуры
            chart.Shapes[0].Text = "Sample CheckBox";
            
            // Сохранить книгу
            workbook.Save("AddShapeInChartWithMsoDrawingType.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


