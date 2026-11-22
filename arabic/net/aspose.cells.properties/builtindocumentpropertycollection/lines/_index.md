---
title: "BuiltInDocumentPropertyCollection.Lines"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تمثل تقديراً لعدد الأسطر في المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/lines/
---
## BuiltInDocumentPropertyCollection.Lines property

تمثل تقديراً لعدد الأسطر في المستند.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Lines { get; set; }
```

### ملاحظات

Aspose.Cells لا يقوم بتحديث هذه الخاصية عندما تقوم بتعديل المستند.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyLinesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // اعرض القيمة الحالية لخاصية Lines (تقدير لعدد الأسطر في المستند)
            Console.WriteLine("Current Lines value: " + properties.Lines);
            
            // عيّن قيمة جديدة لخاصية Lines
            properties.Lines = 150;
            
            // أضف بعض المحتوى لتوضيح غرض الخاصية
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Line " + (i + 1);
            }
            
            // احفظ المصنف
            workbook.Save("PropertyLinesDemo.xlsx");
            
            // ملاحظة: خاصية Lines هي تقدير ولن يتم تحديثها تلقائيًا بالمحتوى الفعلي
            // يُستخدم أساسًا لأغراض بيانات تعريف المستند
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


