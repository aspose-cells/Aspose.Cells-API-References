---
title: "BuiltInDocumentPropertyCollection.DocumentVersion"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تمثل إصدار الملف"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/documentversion/
---
## BuiltInDocumentPropertyCollection.DocumentVersion property

يمثل نسخة الملف.

```csharp
public string DocumentVersion { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyDocumentVersionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // اضبط خاصية إصدار المستند
            workbook.BuiltInDocumentProperties.DocumentVersion = "1.0";
            
            // اعرض إصدار المستند
            Console.WriteLine("Document Version: " + workbook.BuiltInDocumentProperties.DocumentVersion);
            
            // احفظ المصنف
            workbook.Save("DocumentVersionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


