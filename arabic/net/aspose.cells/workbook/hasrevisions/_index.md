---
title: "Workbook.HasRevisions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. يحصل على ما إذا كان دفتر العمل يحتوي على أي تغييرات متتبعة"
type: docs
url: /ar/net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

يحصل على ما إذا كان المصنف يحتوي على أي تغييرات متتبعة

```csharp
public bool HasRevisions { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasRevisionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مع مراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إجراء تغيير سيؤدي إلى إنشاء مراجعة
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // تحقق مما إذا كان المصنف يحتوي على مراجعات
            Console.WriteLine("Workbook has revisions: " + workbook.HasRevisions);
            
            // قبول جميع المراجعات (إن وجدت)
            if (workbook.HasRevisions)
            {
                workbook.AcceptAllRevisions();
            }
            
            // التحقق مرة أخرى بعد قبول المراجعات
            Console.WriteLine("Workbook has revisions after accepting: " + workbook.HasRevisions);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


