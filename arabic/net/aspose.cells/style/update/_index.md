---
title: "Style.Update"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Style. تطبيق النمط المسمى على أنماط الخلايا التي تستخدم هذا النمط المسمى. يعمل كما الضغط على زر موافق بعد الانتهاء من تعديل النمط. ينطبق فقط على النمط المسمى"
type: docs
url: /ar/net/aspose.cells/style/update/
---
## Style.Update method

طبق النمط المسمى على أنماط الخلايا التي تستخدم هذا النمط المسمى. يعمل كما لو قمت بالنقر على زر "ok" بعد الانتهاء من تعديل النمط. يُطبق فقط على النمط المسمى.

```csharp
public void Update()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodUpdateDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نمط
            Style style = workbook.CreateStyle();
            style.Number = 3; // Set to Percent format
            
            // تطبيق النمط على الخلية A1
            worksheet.Cells["A1"].SetStyle(style);
            
            // تعديل النمط
            style.Number = 4; // Change to Currency format
            
            // تحديث تغييرات النمط
            style.Update();
            
            // تحقق من أن النمط تم تحديثه
            Console.WriteLine("Cell A1 Number Format: " + worksheet.Cells["A1"].GetStyle().Number);
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


