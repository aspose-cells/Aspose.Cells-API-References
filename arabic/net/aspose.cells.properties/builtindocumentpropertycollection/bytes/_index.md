---
title: "BuiltInDocumentPropertyCollection.Bytes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تمثّل تقديرًا لعدد البايتات في المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/bytes/
---
## BuiltInDocumentPropertyCollection.Bytes property

تمثّل تقديرًا لعدد البايتات في المستند.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Bytes { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyBytesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // اعرض قيمة Bytes الحالية (تقدير حجم المستند)
            Console.WriteLine("Current Bytes value: " + properties.Bytes);

            // أضف بعض المحتوى لتغيير الحجم
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data to increase document size");
            for (int i = 2; i <= 100; i++)
            {
                worksheet.Cells["A" + i].PutValue("Line " + i);
            }

            // حدّث خاصية Bytes يدويًا (مع أن هذا عادةً يُحسب تلقائيًا)
            properties.Bytes = 5000;
            Console.WriteLine("Updated Bytes value: " + properties.Bytes);

            // احفظ دفتر العمل لرؤية الخاصية في الملف المحفوظ
            workbook.Save("PropertyBytesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


