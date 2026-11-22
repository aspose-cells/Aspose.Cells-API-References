---
title: "DeleteOptions.UpdateReference"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DeleteOptions. تشير إلى ما إذا كان يتم تحديث المراجع في أوراق عمل أخرى"
type: docs
url: /ar/net/aspose.cells/deleteoptions/updatereference/
---
## DeleteOptions.UpdateReference property

يشير إلى ما إذا كان يتم تحديث المراجع في أوراق العمل الأخرى.

```csharp
public bool UpdateReference { get; set; }
```

### ملاحظات

بدءًا من الإصدار 26.7 نضبط القيمة الافتراضية لهذه الخاصية إلى true.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة وصيغ
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // إنشاء خيارات حذف مع تعيين UpdateReference إلى true
            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;

            // حذف العمود A الذي يتم الإشارة إليه في الصيغ
            worksheet.Cells.DeleteColumns(0, 1, deleteOptions);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


