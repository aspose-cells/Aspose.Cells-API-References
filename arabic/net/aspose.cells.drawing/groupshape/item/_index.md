---
title: "GroupShape.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GroupShape. يحصل على الشكل الفرعي حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.drawing/groupshape/item/
---
## GroupShape indexer

يحصل على الشكل الفرعي حسب الفهرس.

```csharp
public Shape this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | فهرس الشكل الفرعي. |

### قيمة الإرجاع

يرجع الشكل الفرعي.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapePropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ شكلين مستطيلين
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // اجمع الأشكال
            Shape[] shapesToGroup = new Shape[] { shape1, shape2 };
            GroupShape groupShape = worksheet.Shapes.Group(shapesToGroup);

            // الوصول وعرض خصائص الشكل الأول
            Shape firstShape = groupShape[0];
            Console.WriteLine($"First shape initial name: {firstShape.Name}");
            Console.WriteLine($"First shape initial text: {firstShape.Text}");

            // تعديل خصائص الشكل الأول عبر الوصول إلى Item
            firstShape.Name = "ModifiedRectangle1";
            firstShape.Text = "First Grouped Shape";

            // الوصول وتعديل الشكل الثاني مباشرة عبر indexer
            groupShape[1].Text = "Second Grouped Shape";

            // تحقق من التغييرات
            Console.WriteLine($"\nFirst shape updated name: {groupShape[0].Name}");
            Console.WriteLine($"First shape updated text: {groupShape[0].Text}");
            Console.WriteLine($"Second shape updated text: {groupShape[1].Text}");

            // حفظ المصنف المعدل
            workbook.Save("GroupShapePropertyItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


