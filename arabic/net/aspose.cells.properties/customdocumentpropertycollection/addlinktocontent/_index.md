---
title: "CustomDocumentPropertyCollection.AddLinkToContent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomDocumentPropertyCollection. تنشئ خاصية مستند مخصصة جديدة ترتبط بالمحتوى"
type: docs
url: /ar/net/aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/
---
## CustomDocumentPropertyCollection.AddLinkToContent method

إنشاء خاصية مستند مخصصة جديدة ترتبط بالمحتوى.

```csharp
public DocumentProperty AddLinkToContent(string name, string source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية. |
| المصدر | String | مصدر الخاصية. يجب أن يكون اسم النطاق المسمى. |

### قيمة الإرجاع

كائن الخاصية الذي تم إنشاؤه حديثًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddLinkToContentWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن قيمة في الخلية A1 سيتم ربطها
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // أضف خاصية عادية للمقارنة
            customProperties.Add("RegularProperty", "Static Value");
            
            // أضف خاصية مرتبطة
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");
            
            // حدّث القيمة المرتبطة
            customProperties.UpdateLinkedRange();

            // اعرض الخصائص
            Console.WriteLine($"Regular Property: {customProperties["RegularProperty"].Value}");
            Console.WriteLine($"Linked Property: {customProperties["LinkedProperty"].Value}");

            workbook.Save("LinkedPropertyExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


