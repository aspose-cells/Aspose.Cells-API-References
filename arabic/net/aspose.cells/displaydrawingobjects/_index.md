---
title: "تعداد DisplayDrawingObjects"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.DisplayDrawingObjects. يمثل ما إذا كان وكيفية إظهار الكائنات في دفتر العمل"
type: docs
url: /ar/net/aspose.cells/displaydrawingobjects/
---
## DisplayDrawingObjects enumeration

يمثل ما إذا كان وكيفية إظهار الكائنات في المصنف.

```csharp
public enum DisplayDrawingObjects
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DisplayShapes | `0` | إظهار جميع الكائنات |
| Placeholders | `1` | إظهار العناصر النائبة |
| Hide | `2` | إخفاء جميع الأشكال. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DisplayDrawingObjectsDemo
    {
        public static void DisplayDrawingObjectsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات دفتر العمل
            WorkbookSettings settings = workbook.Settings;

            // عيّن خاصية DisplayDrawingObjects لإظهار جميع الكائنات
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;

            // احفظ المصنف
            workbook.Save("DisplayDrawingObjectsExample_DisplayShapes.xlsx");

            // عيّن خاصية DisplayDrawingObjects لإظهار العناصر النائبة
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;

            // احفظ المصنف
            workbook.Save("DisplayDrawingObjectsExample_Placeholders.xlsx");

            // عيّن خاصية DisplayDrawingObjects لإخفاء جميع الأشكال
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;

            // احفظ المصنف
            workbook.Save("DisplayDrawingObjectsExample_Hide.xlsx");
            workbook.Save("DisplayDrawingObjectsExample_Hide.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


