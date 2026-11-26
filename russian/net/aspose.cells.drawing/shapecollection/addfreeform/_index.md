---
title: "ShapeCollection.AddFreeform"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет свободноформенную фигуру в лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection.AddFreeform method

Добавляет произвольную форму на лист.

```csharp
public Shape AddFreeform(int topRow, int top, int leftColumn, int left, int height, int width, 
    ShapePath[] paths)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение свободноформенной фигуры от её левой строки в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение свободноформенной фигуры от её левого столбца в пикселях. |
| высота | Int32 | Представляет высоту свободноформенной фигуры в пикселях. |
| ширина | Int32 | Представляет ширину свободноформенной фигуры в пикселях. |
| пути | ShapePath[] | Представляет пользовательский путь |

### Возвращаемое значение

Свободноформенная фигура.

### Примечания

Примечание: Ширина и высота в параметрах могут быть любыми положительными целыми значениями, а не общей шириной и высотой массива ShapePath, указанного в ’paths'. Отношение между ними — масштабно‑заполняющее, то есть каждый объект ShapePath будет масштабироваться в соответствии с указанными шириной и высотой. Поэтому, когда в 'paths' присутствует несколько объектов, каждый объект ShapePath необходимо разумно проектировать, чтобы соответствовать ожиданиям. Если присутствует только один объект ShapePath и нет других требований, передача ширины и высоты объекта в качестве значений параметров является хорошим решением.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeformWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Создать пользовательские пути фигур
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();
            
            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                                96.5f, -7.148871f,
                                130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                                182.24997f, 75.351f,
                                201, 120.517795f);
            shapePath1.MoveTo(150, 80);
            shapePath1.ArcTo(25, 25, 0, 270);
            
            // Добавить свободноформенную фигуру в лист
            shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath, shapePath1 });

            // Сохраните книгу
            workbook.Save("AddFreeformDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* class [ShapePath](../../shapepath/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


