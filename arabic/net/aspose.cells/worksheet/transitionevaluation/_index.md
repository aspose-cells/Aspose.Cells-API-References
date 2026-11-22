---
title: "Worksheet.TransitionEvaluation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Worksheet property. يشير إلى ما إذا كان خيار توافق Lotus لتقييم صيغة الانتقال مفعلًا"
type: docs
url: /ar/net/aspose.cells/worksheet/transitionevaluation/
---
## Worksheet.TransitionEvaluation property

يشير إلى ما إذا كان خيار تقييم الصيغة الانتقالية (توافق Lotus) مفعلاً.

```csharp
public bool TransitionEvaluation { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEvaluationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين خاصية TransitionEvaluation
            worksheet.TransitionEvaluation = true;
            
            // عرض قيمة الخاصية
            Console.WriteLine("TransitionEvaluation: " + worksheet.TransitionEvaluation);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // حمّل دفتر العمل المحفوظ للتحقق من الخاصية
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("Loaded TransitionEvaluation: " + loadedWorksheet.TransitionEvaluation);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


