---
title: "WorkbookSettings.DiscardImageEditData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان يتم تجاهل بيانات تحرير الصورة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/discardimageeditdata/
---
## WorkbookSettings.DiscardImageEditData property

يشير إلى ما إذا كان يتم تجاهل بيانات تحرير الصورة.

```csharp
public bool DiscardImageEditData { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDiscardImageEditDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة صورة إلى ورقة العمل
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // تعيين DiscardImageEditData إلى true (القيمة الافتراضية هي false)
            workbook.Settings.DiscardImageEditData = true;
            
            // احفظ المصنف
            workbook.Save("output_with_discarded_image_data.xlsx", SaveFormat.Xlsx);
            
            // تحقق من تطبيق الإعداد
            Console.WriteLine("DiscardImageEditData is set to: " + workbook.Settings.DiscardImageEditData);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


