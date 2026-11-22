---
title: "Range.Transpose"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تقوم Transpose بتدوير البيانات من الصفوف إلى الأعمدة أو العكس"
type: docs
url: /ar/net/aspose.cells/range/transpose/
---
## Range.Transpose method

نقل (تدوير) البيانات من الصفوف إلى الأعمدة أو العكس.

```csharp
public void Transpose()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodTransposeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بيانات عينة في نطاق 3x3 (A1:C3)
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].PutValue(6);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["C3"].PutValue(9);
            
            // إنشاء نطاق (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            
            // تدوير النطاق
            range.Transpose();
            
            // احفظ المصنف
            workbook.Save("TransposedOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


