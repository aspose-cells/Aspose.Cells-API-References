---
title: "ShapeCollection.AddSpinner"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تُضيف Spinner إلى ورقة العمل."
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addspinner/
---
## ShapeCollection.AddSpinner method

يضيف Spinner إلى ورقة العمل.

```csharp
public Spinner AddSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| أعلى | Int32 | يمثل الإزاحة العمودية لـ Spinner من صفه الأيسر بوحدة البكسل. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| يسار | Int32 | يمثل الإزاحة الأفقية لـ Spinner من عموده الأيسر بوحدة البكسل. |
| الارتفاع | Int32 | يمثل ارتفاع Spinner بوحدة البكسل. |
| العرض | Int32 | يمثل عرض Spinner بوحدة البكسل. |

### قيمة الإرجاع

كائن Spinner.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSpinnerWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة Spinner إلى ورقة العمل.
            Aspose.Cells.Drawing.Spinner spinner = (Aspose.Cells.Drawing.Spinner)worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 50);

            // اضبط خصائص Spinner
            spinner.LinkedCell = "A1";
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 1;

            // احفظ المصنف
            workbook.Save("AddSpinnerDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Spinner](../../spinner/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


