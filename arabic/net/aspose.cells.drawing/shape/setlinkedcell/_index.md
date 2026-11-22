---
title: "Shape.SetLinkedCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تعيين النطاق المرتبط بقيمة التحكم"
type: docs
url: /ar/net/aspose.cells.drawing/shape/setlinkedcell/
---
## Shape.SetLinkedCell method

يضبط النطاق المرتبط بقيمة التحكم.

```csharp
public void SetLinkedCell(string formula, bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | النطاق المرتبط بقيمة التحكم. |
| isR1C1 | منطقي | ما إذا كان يجب تنسيق الصيغة كـ R1C1. |
| isLocal | منطقي | ما إذا كان يجب تنسيق الصيغة وفقًا للمنطقة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLinkedCellWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل شريط تمرير
            Aspose.Cells.Drawing.Shape scrollBar = worksheet.Shapes.AddScrollBar(2, 0, 2, 0, 130, 30);

            // ربط قيمة شريط التمرير بالخلية A12
            scrollBar.SetLinkedCell("$A$12", false, true);

            // احفظ المصنف
            workbook.Save("SetLinkedCellDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


