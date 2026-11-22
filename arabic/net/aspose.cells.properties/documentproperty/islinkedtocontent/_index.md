---
title: "DocumentProperty.IsLinkedToContent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocumentProperty. تشير إلى ما إذا كانت هذه الخاصية مرتبطة بالمحتوى"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/islinkedtocontent/
---
## DocumentProperty.IsLinkedToContent property

يشير إلى ما إذا كانت هذه الخاصية مرتبطة بالمحتوى

```csharp
public bool IsLinkedToContent { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyIsLinkedToContentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بيانات تجريبية إلى الخلايا
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Company Name";
            worksheet.Cells["B1"].Value = "Company Address";

            // أنشئ خصائص مستند مخصصة مرتبطة
            workbook.CustomDocumentProperties.AddLinkToContent("Company", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Address", "B1");

            // احصل على خاصية IsLinkedToContent وتحقق منها
            DocumentProperty companyProp = workbook.CustomDocumentProperties["Company"];
            Console.WriteLine($"Is 'Company' property linked to content: {companyProp.IsLinkedToContent}");
            Console.WriteLine($"Linked source: {companyProp.Source}");
            Console.WriteLine($"Current value: {companyProp.Value}");

            // حدّث قيمة الخلية وقم بتحديث الخصائص المرتبطة
            worksheet.Cells["A1"].Value = "Updated Company Name";
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // تحقق من أن الخاصية تم تحديثها
            Console.WriteLine($"Updated value: {companyProp.Value}");

            // احفظ المصنف
            workbook.Save("LinkedPropertiesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


