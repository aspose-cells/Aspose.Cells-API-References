---
title: "التعداد ShapePathPointValueType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.ShapePathPointValueType. يحدد نوع القيمة لكائن ShapePathPoint"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathpointvaluetype/
---
## ShapePathPointValueType enumeration

يحدد نوع القيمة لكائن [`ShapePathPoint`](../shapepathpoint/)

```csharp
public enum ShapePathPointValueType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Position | `0` | يحدد نوع الكائن كإحداثيات الموقع. كائن [`ShapePathPoint`](../shapepathpoint/) يخزن قيم إحداثيات نقطة. |
| Angle | `1` | يحدد نوع الكائن كعلامات الزاوية. كائن [`ShapePathPoint`](../shapepathpoint/) يخزن زاوية البداية والنهاية للقوس. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointValueTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // اعرض قيم تعداد ShapePathPointValueType
                ShapePathPointValueType positionType = ShapePathPointValueType.Position;
                ShapePathPointValueType angleType = ShapePathPointValueType.Angle;

                // عرض قيم التعداد
                Console.WriteLine($"Position type value: {(int)positionType}");
                Console.WriteLine($"Angle type value: {(int)angleType}");

                // تحقق من أن قيم التعداد تطابق الثوابت المتوقعة
                Console.WriteLine($"Position equals 0: {positionType == ShapePathPointValueType.Position}");
                Console.WriteLine($"Angle equals 1: {angleType == ShapePathPointValueType.Angle}");

                Console.WriteLine("ShapePathPointValueType enum demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPointValueType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


