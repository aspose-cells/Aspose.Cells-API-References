---
title: "CustomProperty.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomProperty. تُرجع أو تُحدد قيمة الخاصية المخصصة"
type: docs
url: /ar/net/aspose.cells.properties/customproperty/value/
---
## CustomProperty.Value property

تُعيد أو تُعيّن قيمة الخاصية المخصصة.

```csharp
public string Value { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة خاصية مخصصة بقيمة نصية طويلة
            worksheet.CustomProperties.Add("VeryLongString", "This is a very long string value for testing custom properties");
            
            // الحصول على قيمة الخاصية المخصصة وعرضها
            string propertyValue = worksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Custom Property Value: " + propertyValue);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // إعادة تحميل المصنف للتحقق من بقاء الخاصية
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // تحقق من أن القيمة هي نفسها بعد التحميل
            string loadedValue = loadedWorksheet.CustomProperties["VeryLongString"].Value;
            Console.WriteLine("Reloaded Custom Property Value: " + loadedValue);
        }
    }
}
```

### انظر أيضًا

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


