---
title: "DocumentProperty.IsGeneratedName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocumentProperty. تُعيد true إذا لم يكن لهذه الخاصية اسم في تخزين OLE2 وتم إنشاء اسم فريد فقط لواجهة برمجة التطبيقات العامة"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/isgeneratedname/
---
## DocumentProperty.IsGeneratedName property

يعيد true إذا لم يكن لهذه الخاصية اسم في تخزين OLE2 وتم إنشاء اسم فريد فقط لواجهة برمجة التطبيقات العامة.

```csharp
public bool IsGeneratedName { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyPropertyIsGeneratedNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خصائص المستند المدمجة
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;
            
            // الوصول إلى خصائص المستند المخصصة للإضافة
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // إضافة خاصية مخصصة
            DocumentProperty customProperty = customProperties.Add("CustomProperty", "Test Value");
            
            // اعرض IsGeneratedName للخاصية المدمجة
            DocumentProperty authorProperty = properties["Author"];
            Console.WriteLine("Author property IsGeneratedName: " + authorProperty.IsGeneratedName);
            
            // اعرض IsGeneratedName للخاصية المخصصة
            Console.WriteLine("Custom property IsGeneratedName: " + customProperty.IsGeneratedName);

            // أنشئ سيناريوً حيث قد تكون للخاصية اسم مُولد
            // (ملاحظة: في الواقع، IsGeneratedName للقراءة فقط ويتم تعيينه داخليًا بواسطة Aspose.Cells)
            DocumentProperty generatedNameProperty = properties["_PID_GUID"];
            if (generatedNameProperty != null)
            {
                Console.WriteLine("Generated name property IsGeneratedName: " + generatedNameProperty.IsGeneratedName);
            }

            // احفظ المصنف
            workbook.Save("PropertyIsGeneratedNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


