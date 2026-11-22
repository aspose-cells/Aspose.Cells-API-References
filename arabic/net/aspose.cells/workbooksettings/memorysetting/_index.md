---
title: "WorkbookSettings.MemorySetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. يحصل أو يضبط خيارات استخدام الذاكرة. سيتم أخذ الخيار الجديد كخيار افتراضي للأوراق العمل التي تم إنشاؤها حديثًا لكنه لا يؤثر على الأوراق الموجودة"
type: docs
url: /ar/net/aspose.cells/workbooksettings/memorysetting/
---
## WorkbookSettings.MemorySetting property

يحصل أو يضبط خيارات استخدام الذاكرة. سيتم اعتبار الخيار الجديد كخيار افتراضي للأوراق العمل التي تم إنشاؤها حديثًا لكنه لا يؤثر على الأوراق الموجودة.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### ملاحظات

لمزيد من التفاصيل حول وضع الذاكرة، يرجى الاطلاع على [`MemorySetting`](../../cells/memorysetting/).

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع إعداد تفضيل الذاكرة
            Workbook wb = new Workbook();
            wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
            
            // الوصول إلى الورقة الأولى وإضافة بعض البيانات
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Memory Setting Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // حفظ إلى تدفق الذاكرة بصيغة PDF
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Pdf);
                Console.WriteLine("Workbook saved to PDF with MemoryPreference setting");
            }
        }
    }
}
```

### انظر أيضًا

* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


