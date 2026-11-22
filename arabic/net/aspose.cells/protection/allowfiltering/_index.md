---
title: "Protection.AllowFiltering"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان يُسمح للمستخدم باستخدام AutoFilter تم إنشاؤه قبل حماية الورقة"
type: docs
url: /ar/net/aspose.cells/protection/allowfiltering/
---
## Protection.AllowFiltering property

يمثل ما إذا كان يُسمح للمستخدم باستخدام الفلتر التلقائي الذي تم إنشاؤه قبل حماية الورقة.

```csharp
public bool AllowFiltering { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFilteringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تمكين حماية ورقة العمل
            worksheet.Protect(ProtectionType.All);
            
            // عيّن خاصية AllowFiltering إلى true
            worksheet.Protection.AllowFiltering = true;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحقق من أن الخاصية تم حفظها بشكل صحيح
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AllowFiltering: " + 
                loadedWorkbook.Worksheets[0].Protection.AllowFiltering);
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


