---
title: "CustomDocumentPropertyCollection.UpdateLinkedRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomDocumentPropertyCollection. تقوم بتحديث جميع النطاقات المرتبطة بالخصائص المخصصة باستخدام قيمة الخاصية المخصصة لتحديث قيمة الخلية للنطاق المرتبط"
type: docs
url: /ar/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/
---
## CustomDocumentPropertyCollection.UpdateLinkedRange method

تحديث جميع النطاقات المرتبطة بالخصائص المخصصة (استخدام قيمة الخاصية المخصصة لتحديث قيمة الخلية للنطاق المرتبط).

```csharp
public void UpdateLinkedRange()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن قيمة في الخلية A1 سيتم ربطها
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // أضف خاصية مرتبطة
            customProperties.AddLinkToContent("LinkedRange", "Sheet1!A1");
            
            // تحديث جميع الخصائص المرتبطة
            customProperties.UpdateLinkedRange();
            
            // الحصول على قيمة الخاصية المرتبطة وعرضها
            DocumentProperty linkedProp = customProperties["LinkedRange"];
            Console.WriteLine($"Linked Property Value: {linkedProp.Value}");

            // احفظ المصنف
            workbook.Save("LinkedRangeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


