---
title: "BuiltInDocumentPropertyCollection.Characters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تمثل تقديراً لعدد الأحرف في المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/characters/
---
## BuiltInDocumentPropertyCollection.Characters property

تمثل تقديراً لعدد الأحرف في المستند.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Characters { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyCharactersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // اعرض قيمة Characters الحالية (خاصية قديمة)
            Console.WriteLine("Current Characters value: " + properties.Characters);

            // اضبط قيمة جديدة لـ Characters (خاصية قديمة)
            properties.Characters = 1500;
            Console.WriteLine("Updated Characters value: " + properties.Characters);

            // أضف بعض المحتوى لتوضيح تأثير الخاصية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample text to demonstrate document properties.");
            
            // احفظ المصنف
            workbook.Save("PropertyCharactersDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


