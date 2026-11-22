---
title: "DocumentProperty.ToInt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DocumentProperty. تُرجع قيمة الخاصية كعدد صحيح"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/toint/
---
## DocumentProperty.ToInt method

يعيد قيمة الخاصية كعدد صحيح.

```csharp
public int ToInt()
```

### ملاحظات

يرمي استثناءً إذا كان نوع الخاصية ليس PropertyType.Number.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToIntDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // احصل على مجموعة خصائص المستند المخصصة
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // أضف خاصية مخصصة رقمية
            customProperties.Add("Revision", 5);

            // احصل على الخاصية وحولها إلى int باستخدام ToInt()
            DocumentProperty revisionProperty = customProperties["Revision"];
            int revisionValue = revisionProperty.ToInt();
            
            // أخرج النتيجة.
            Console.WriteLine($"Revision (as int): {revisionValue}");

            // احفظ المصنف
            workbook.Save("DocumentPropertyToIntExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


