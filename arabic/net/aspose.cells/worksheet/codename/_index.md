---
title: "Worksheet.CodeName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل على اسم رمز الورقة"
type: docs
url: /ar/net/aspose.cells/worksheet/codename/
---
## Worksheet.CodeName property

يحصل على اسم رمز ورقة العمل.

```csharp
public string CodeName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCodeNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عرض اسم الرمز الافتراضي
            Console.WriteLine("Default CodeName: " + worksheet.CodeName);
            
            // تغيير اسم الرمز
            worksheet.CodeName = "MySheet";
            Console.WriteLine("Modified CodeName: " + worksheet.CodeName);
            
            // إضافة ورقة عمل جديدة وعرض اسم الرمز الخاص بها
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            Console.WriteLine("New Sheet CodeName: " + newSheet.CodeName);
            
            // احفظ المصنف
            workbook.Save("WorksheetCodeNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


