---
title: "BuiltInDocumentPropertyCollection.ScaleCrop"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تشير إلى وضع عرض صورة المصغرة للمستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/scalecrop/
---
## BuiltInDocumentPropertyCollection.ScaleCrop property

يشير إلى وضع عرض صورة المصغرة للمستند.

```csharp
public bool ScaleCrop { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyScaleCropDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // تعيين خاصية ScaleCrop
            properties.ScaleCrop = true;
            
            // عرض قيمة خاصية ScaleCrop
            Console.WriteLine("ScaleCrop property value: " + properties.ScaleCrop);
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


