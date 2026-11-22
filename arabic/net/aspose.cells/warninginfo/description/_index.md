---
title: "WarningInfo.Description"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WarningInfo. الحصول على وصف معلومات التحذير"
type: docs
url: /ar/net/aspose.cells/warninginfo/description/
---
## WarningInfo.Description property

احصل على وصف معلومات التحذير.

```csharp
public string Description { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyDescriptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء اسم معرف مكرر لتفعيل التحذير
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA";
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA"; // Different name to actually trigger warning

            // الحصول على رد النداء للتحذير
            WarningCallback callback = new WarningCallback();
            workbook.Settings.WarningCallback = callback; // Correct property path

            // احفظ لتفعيل التحذير
            workbook.Save("output.xlsx");

            // عرض استخدام خاصية Description
            if (callback.LastWarning != null)
            {
                Console.WriteLine("Warning Description: " + callback.LastWarning.Description);
                Console.WriteLine("Warning Type: " + callback.LastWarning.Type);
            }
        }
    }

    public class WarningCallback : IWarningCallback
    {
        public WarningInfo LastWarning { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            LastWarning = warningInfo;
        }
    }
}
```

### انظر أيضًا

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


