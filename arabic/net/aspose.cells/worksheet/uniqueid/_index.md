---
title: "Worksheet.UniqueId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل وتعيّن المعرف الفريد وهو نفسه 15DB5C3CA5A148AF8F253D86AC232D4F"
type: docs
url: /ar/net/aspose.cells/worksheet/uniqueid/
---
## Worksheet.UniqueId property

يحصل على ويضبط المعرف الفريد، وهو نفسه {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

```csharp
public string UniqueId { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyUniqueIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء معرف فريد للورقة
            string uniqueId = "{" + Guid.NewGuid().ToString() + "}";
            
            // تعيين خاصية UniqueId للورقة الأولى
            workbook.Worksheets[0].UniqueId = uniqueId;
            
            // احفظ المصنف
            string outputPath = "SheetUniqueIdDemo.xlsx";
            workbook.Save(outputPath);
            
            // إعادة تحميل المصنف للتحقق من بقاء UniqueId
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // إخراج UniqueId لإظهار الوظيفة
            Console.WriteLine("Worksheet UniqueId: " + loadedWorkbook.Worksheets[0].UniqueId);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


