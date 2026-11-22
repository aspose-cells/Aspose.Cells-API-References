---
title: "Worksheet.TabId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحدد المعرف الداخلي للورقة"
type: docs
url: /ar/net/aspose.cells/worksheet/tabid/
---
## Worksheet.TabId property

يحدد المعرف الداخلي للورقة.

```csharp
public int TabId { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين خاصية TabId
            worksheet.TabId = 107;
            
            // احفظ المصنف
            string outputPath = "output.xlsb";
            workbook.Save(outputPath);
            
            // تحميل المصنف المحفوظ للتحقق من TabId
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // عرض قيمة TabId
            Console.WriteLine("Worksheet TabId: " + loadedWorksheet.TabId);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


