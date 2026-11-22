---
title: "DocumentProperty.ToDouble"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DocumentProperty. تُرجع قيمة الخاصية كعدد مزدوج"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/todouble/
---
## DocumentProperty.ToDouble method

يعيد قيمة الخاصية كقيمة مزدوجة.

```csharp
public double ToDouble()
```

### ملاحظات

يرمي استثناءً إذا لم يكن نوع الخاصية PropertyType.Float.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToDoubleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // احصل على مجموعة خصائص المستند المخصصة
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // أضف خاصية رقمية
            customProperties.Add("Rating", 4.75);

            // احصل على الخاصية وحوّلها إلى مزدوج
            DocumentProperty ratingProperty = customProperties["Rating"];
            double ratingValue = ratingProperty.ToDouble();

            // أخرج النتيجة.
            Console.WriteLine($"Rating: {ratingValue}");

            // احفظ المصنف
            workbook.Save("DocumentPropertyToDoubleExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


