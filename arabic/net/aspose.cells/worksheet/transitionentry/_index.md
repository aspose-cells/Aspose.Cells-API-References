---
title: "Worksheet.TransitionEntry"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تشير إلى ما إذا كان خيار التوافق مع Lotus لـ Transition Formula Entry مُفعّلاً"
type: docs
url: /ar/net/aspose.cells/worksheet/transitionentry/
---
## Worksheet.TransitionEntry property

يشير إلى ما إذا كان خيار إدخال الصيغة الانتقالية (توافق Lotus) مفعلاً.

```csharp
public bool TransitionEntry { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEntryDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن خاصية TransitionEntry
            worksheet.TransitionEntry = true;
            
            // اعرض قيمة TransitionEntry
            Console.WriteLine("TransitionEntry: " + worksheet.TransitionEntry);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // حمّل دفتر العمل المحفوظ للتحقق من الخاصية
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // اعرض قيمة TransitionEntry المحمّلة
            Console.WriteLine("Loaded TransitionEntry: " + loadedWorksheet.TransitionEntry);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


