---
title: "WriteProtection.RecommendReadOnly"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WriteProtection. تشير إلى ما إذا تم اختيار خيار القراءة فقط الموصى به"
type: docs
url: /ar/net/aspose.cells/writeprotection/recommendreadonly/
---
## WriteProtection.RecommendReadOnly property

يشير إلى ما إذا تم اختيار خيار القراءة فقط الموصى به.

```csharp
public bool RecommendReadOnly { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyRecommendReadOnlyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل وإضافة بعض بيانات العينة
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // عيّن RecommendReadOnly إلى true
            workbook.Settings.WriteProtection.RecommendReadOnly = true;
            
            // تحقق من تعيين الخاصية
            Console.WriteLine("RecommendReadOnly: " + workbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("IsWriteProtected: " + workbook.Settings.WriteProtection.IsWriteProtected);

            // احفظ المصنف
            workbook.Save("output_recommend_readonly.xlsx");

            // حمّل المصنف المحفوظ للتحقق من بقاء الإعدادات
            Workbook loadedWorkbook = new Workbook("output_recommend_readonly.xlsx");
            Console.WriteLine("After loading - RecommendReadOnly: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("After loading - IsWriteProtected: " + loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### انظر أيضًا

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


