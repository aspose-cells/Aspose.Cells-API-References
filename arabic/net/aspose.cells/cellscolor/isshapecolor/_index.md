---
title: "CellsColor.IsShapeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsColor. الحصول على اللون وتعيينه الذي يجب تطبيقه على الخلية أو الشكل"
type: docs
url: /ar/net/aspose.cells/cellscolor/isshapecolor/
---
## CellsColor.IsShapeColor property

يحصل على اللون ويضبطه الذي يجب تطبيقه على الخلية أو الشكل.

```csharp
public bool IsShapeColor { get; set; }
```

### ملاحظات

تعبير اللون للخلية والشكل مختلف. على سبيل المثال: لون السمة بنفس قيمة الصبغة لن يكون هو نفسه في الخلية والشكل.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyIsShapeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مثيل CellsColor وتعيين IsShapeColor
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.IsShapeColor = true;
            cellsColor.Color = Color.Green;

            // تطبيق اللون على شكل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = cellsColor.Color;  // Use the Color property instead of CellsColor directly

            // احفظ المصنف
            workbook.Save("CellsColorIsShapeColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


