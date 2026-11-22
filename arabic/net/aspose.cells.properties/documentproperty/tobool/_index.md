---
title: "DocumentProperty.ToBool"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DocumentProperty. تُرجع قيمة الخاصية كقيمة منطقية"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/tobool/
---
## DocumentProperty.ToBool method

يعيد قيمة الخاصية كقيمة منطقية.

```csharp
public bool ToBool()
```

### ملاحظات

يرمي استثناءً إذا لم يكن نوع الخاصية PropertyType.Boolean.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyMethodToBoolDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // أضف خاصية مستند مخصصة منطقية
            customProperties.Add("IsApproved", true);
            
            // احصل على الخاصية وحوّلها إلى قيمة منطقية باستخدام ToBool()
            DocumentProperty isApprovedProperty = customProperties["IsApproved"];
            bool isApproved = isApprovedProperty.ToBool();
            
            Console.WriteLine($"Is Approved: {isApproved}");
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


