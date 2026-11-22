---
title: "GroupShape.Ungroup"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GroupShape. تفك تجميع عناصر الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/groupshape/ungroup/
---
## GroupShape.Ungroup method

فك تجميع عناصر الشكل.

```csharp
public void Ungroup()
```

### ملاحظات

إذا كان شكل التجميع مُجَمَّعًا بواسطة شكل تجميع آخر، لن يتم تنفيذ أي شيء.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapeMethodUngroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلين مستطيلين
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 50);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 3, 0, 100, 50);

            // اجمع الأشكال في GroupShape
            GroupShape groupShape = worksheet.Shapes.Group(new Shape[] { shape1, shape2 });

            try
            {
                // نفّذ طريقة Ungroup
                groupShape.Ungroup();
                Console.WriteLine("Shapes ungrouped successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ungrouping: {ex.Message}");
            }

            workbook.Save("GroupShapeUngroupDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


