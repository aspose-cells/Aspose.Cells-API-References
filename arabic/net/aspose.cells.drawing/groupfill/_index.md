---
title: "فئة GroupFill"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Drawing.GroupFill. تمثل أن تنسيق التعبئة هذا يجب أن يرث خصائص التعبئة للمجموعة"
type: docs
url: /ar/net/aspose.cells.drawing/groupfill/
---
## GroupFill class

يمثل أن تنسيق التعبئة هذا يجب أن يرث خصائص التعبئة للمجموعة.

```csharp
public class GroupFill : Fill
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(موروث من [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | الحصول على رمز التجزئة. (موروث من [`Fill`](../fill/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGroupFillDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للتوضيح
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GroupFill لا تعرض مُنشئًا عامًا بدون معلمات.
                // لأغراض التوضيح نحصل على مرجع (null) من النوع.
                GroupFill groupFill = null;

                // أظهر أن المتغير من النوع GroupFill موجود.
                Console.WriteLine($"GroupFill variable declared. Type: {typeof(GroupFill).FullName}");

                // احفظ المصنف (على الرغم من أننا لم نقم بتعديله، هذا يُظهر سير عمل كامل)
                workbook.Save("GroupFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GroupFill: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


