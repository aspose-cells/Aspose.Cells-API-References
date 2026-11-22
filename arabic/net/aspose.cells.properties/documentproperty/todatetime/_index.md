---
title: "DocumentProperty.ToDateTime"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DocumentProperty. تُعيد قيمة الخاصية كـ DateTime في المنطقة الزمنية المحلية"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/todatetime/
---
## DocumentProperty.ToDateTime method

يعيد قيمة الخاصية كـ DateTime في المنطقة الزمنية المحلية.

```csharp
public DateTime ToDateTime()
```

### ملاحظات

يرمي استثناءً إذا لم يكن نوع الخاصية PropertyType.Date.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDateTimeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // احصل على مجموعة خصائص المستند المخصصة
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // أضف خاصية datetime
            DateTime currentTime = DateTime.Now;
            customProperties.Add("LastModified", currentTime);

            // احصل على الخاصية وحولها إلى DateTime
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DateTime retrievedTime = lastModifiedProperty.ToDateTime();

            // أخرج النتيجة.
            Console.WriteLine($"Stored DateTime: {currentTime}");
            Console.WriteLine($"Retrieved DateTime: {retrievedTime}");

            // احفظ المصنف
            workbook.Save("DocumentPropertyDateTimeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


