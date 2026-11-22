---
title: "Worksheet.IsProtected"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تشير إلى ما إذا كانت ورقة العمل محمية"
type: docs
url: /ar/net/aspose.cells/worksheet/isprotected/
---
## Worksheet.IsProtected property

يشير إلى ما إذا كانت ورقة العمل محمية.

```csharp
public bool IsProtected { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // حماية المصنف والورقة الأولى
            workbook.Protect(ProtectionType.All, "password");
            workbook.Worksheets[0].Protect(ProtectionType.All, "password", null);

            // تحقق مما إذا كانت ورقة العمل محمية
            bool isProtected = workbook.Worksheets[0].IsProtected;
            Console.WriteLine($"Worksheet is protected: {isProtected}");

            // احفظ المصنف
            workbook.Save("protected_worksheet.xlsx");

            // حمّل دفتر العمل المحفوظ وتحقق من الحماية
            Workbook loadedWorkbook = new Workbook("protected_worksheet.xlsx");
            Console.WriteLine($"Loaded worksheet is protected: {loadedWorkbook.Worksheets[0].IsProtected}");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


