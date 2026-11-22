---
title: "WorkbookSettings.RemovePersonalInformation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. true إذا كان يمكن إزالة المعلومات الشخصية من المصنف المحدد"
type: docs
url: /ar/net/aspose.cells/workbooksettings/removepersonalinformation/
---
## WorkbookSettings.RemovePersonalInformation property

صحيح إذا كان يمكن إزالة المعلومات الشخصية من المصنف المحدد.

```csharp
public bool RemovePersonalInformation { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تعيين RemovePersonalInformation إلى true
            workbook.Settings.RemovePersonalInformation = true;
            
            // أضف بعض البيانات التجريبية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Email");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue("john@example.com");
            
            // احفظ المصنف
            string outputPath = "output_with_personal_info_removed.xlsx";
            workbook.Save(outputPath);
            
            // تحميل الدفتر المحفوظ للتحقق من الإعداد
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("RemovePersonalInformation setting: " + 
                loadedWorkbook.Settings.RemovePersonalInformation);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


