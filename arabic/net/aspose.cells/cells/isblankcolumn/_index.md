---
title: "Cells.IsBlankColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تتحقق مما إذا كان العمود المحدد فارغًا ولا يحتوي على أي بيانات"
type: docs
url: /ar/net/aspose.cells/cells/isblankcolumn/
---
## Cells.IsBlankColumn method

يتحقق مما إذا كان العمود المحدد فارغًا (لا يحتوي على أي بيانات).

```csharp
public bool IsBlankColumn(int columnIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود |

### قيمة الإرجاع

صحيح إذا كان العمود المحدد لا يحتوي على أي بيانات

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsBlankColumnWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحقق مما إذا كان العمود 2 فارغًا (يجب أن يكون صحيحًا لورقة عمل جديدة)
            Console.WriteLine("Is column 2 blank? " + worksheet.Cells.IsBlankColumn(1));

            // أضف بيانات إلى العمود 2
            worksheet.Cells["B1"].PutValue("Test Data");

            // تحقق مرة أخرى (يجب أن يكون الآن خطأ)
            Console.WriteLine("Is column 2 blank after adding data? " + worksheet.Cells.IsBlankColumn(1));

            // إنشاء ورقة عمل أخرى بأعمدة فارغة تمامًا
            Worksheet worksheet2 = workbook.Worksheets.Add("BlankSheet");

            // تحقق من عمود في ورقة العمل الفارغة (يجب أن يكون صحيحًا)
            Console.WriteLine("Is column 3 blank in new sheet? " + worksheet2.Cells.IsBlankColumn(2));
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


