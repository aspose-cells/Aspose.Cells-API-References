---
title: "Cells.StandardWidthInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصّل أو تعيّن عرض العمود الافتراضي في ورقة العمل بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells/cells/standardwidthinch/
---
## Cells.StandardWidthInch property

يحصل أو يعيّن عرض العمود الافتراضي في ورقة العمل، بوحدة البوصة.

```csharp
public double StandardWidthInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين عرض العمود القياسي بالبوصة
            worksheet.Cells.StandardWidthInch = 1.5;

            // تعيين عرض عمود محدد بالبوصة للتجربة
            worksheet.Cells.SetColumnWidthInch(1, 2.0);

            // احفظ المصنف
            workbook.Save("StandardWidthInchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


