---
title: "CustomDocumentPropertyCollection.UpdateLinkedPropertyValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomDocumentPropertyCollection. تقوم بتحديث قيم جميع الخصائص المخصصة المرتبطة بالمحتوى باستخدام قيمة الخلية للنطاق المرتبط لتحديث قيمة الخاصية المخصصة"
type: docs
url: /ar/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/
---
## CustomDocumentPropertyCollection.UpdateLinkedPropertyValue method

تحديث قيم جميع الخصائص المخصصة المرتبطة بالمحتوى (استخدام قيمة الخلية للنطاق المرتبط لتحديث قيمة الخاصية المخصصة).

```csharp
public void UpdateLinkedPropertyValue()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض البيانات إلى الخلايا التي سيتم ربطها بالخصائص المخصصة
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "InitialValue1";
            worksheet.Cells["B1"].Value = "InitialValue2";

            // أضف خصائص مخصصة مرتبطة
            workbook.CustomDocumentProperties.AddLinkToContent("CompanyName", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Department", "B1");

            // حدّث قيم الخلايا
            worksheet.Cells["A1"].Value = "UpdatedValue1";
            worksheet.Cells["B1"].Value = "UpdatedValue2";

            // حدّث قيم الخصائص المرتبطة
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // اعرض قيم الخصائص المحدثة
            Console.WriteLine("CompanyName: " + workbook.CustomDocumentProperties["CompanyName"].Value);
            Console.WriteLine("Department: " + workbook.CustomDocumentProperties["Department"].Value);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


