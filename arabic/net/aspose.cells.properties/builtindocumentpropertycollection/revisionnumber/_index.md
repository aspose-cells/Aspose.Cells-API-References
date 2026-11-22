---
title: "BuiltInDocumentPropertyCollection.RevisionNumber"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تحصل أو تعين رقم مراجعة المستند"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/revisionnumber/
---
## BuiltInDocumentPropertyCollection.RevisionNumber property

يحصل أو يضبط رقم مراجعة المستند.

```csharp
public string RevisionNumber { get; set; }
```

### ملاحظات

Aspose.Cells لا يقوم بتحديث هذه الخاصية عندما تقوم بتعديل المستند.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyRevisionNumberDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // عيّن خاصية RevisionNumber
            workbook.BuiltInDocumentProperties.RevisionNumber = "1";
            
            // اعرض RevisionNumber
            Console.WriteLine("Revision Number: " + workbook.BuiltInDocumentProperties.RevisionNumber);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


