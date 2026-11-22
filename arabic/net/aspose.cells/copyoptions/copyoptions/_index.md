---
title: "CopyOptions.CopyOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ CopyOptions. منشئ CopyOptions"
type: docs
url: /ar/net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

منشئ CopyOptions.

```csharp
public CopyOptions()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل والحصول على ورقة العمل الأولى
            Worksheet sourceSheet = workbook.Worksheets[0];
            Worksheet destSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            
            // إضافة بيانات نموذجية إلى الورقة المصدر
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            sourceSheet.Cells["A4"].PutValue(300);
            
            // إنشاء CopyOptions باستخدام المنشئ
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;
            
            // نسخ الصفوف باستخدام الخيارات
            destSheet.Cells.CopyRows(sourceSheet.Cells, 0, 0, sourceSheet.Cells.MaxDisplayRange.RowCount, options);
            
            // احفظ المصنف
            workbook.Save("CopyOptionsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


