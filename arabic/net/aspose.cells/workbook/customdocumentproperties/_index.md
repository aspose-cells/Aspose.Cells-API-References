---
title: "Workbook.CustomDocumentProperties"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تُعيد مجموعة DocumentProperty التي تمثل جميع خصائص المستند المخصصة للجدول الإلكتروني"
type: docs
url: /ar/net/aspose.cells/workbook/customdocumentproperties/
---
## Workbook.CustomDocumentProperties property

تُرجع مجموعة [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) تمثل جميع خصائص المستند المخصصة لجدول البيانات.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة خصائص مستند مخصصة
            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Created Date", DateTime.Now);
            workbook.CustomDocumentProperties.Add("Revision", 1);
            workbook.CustomDocumentProperties.Add("Approved", true);
            
            // الوصول وعرض الخصائص المخصصة
            Console.WriteLine("Custom Document Properties:");
            foreach (Aspose.Cells.Properties.DocumentProperty prop in workbook.CustomDocumentProperties)
            {
                Console.WriteLine($"{prop.Name}: {prop.Value} ({prop.Type})");
            }
            
            // احفظ المصنف
            workbook.Save("CustomDocumentPropertiesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


