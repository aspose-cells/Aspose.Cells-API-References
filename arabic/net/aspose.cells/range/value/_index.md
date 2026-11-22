---
title: "Range.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل أو يضبط قيمة النطاق"
type: docs
url: /ar/net/aspose.cells/range/value/
---
## Range.Value property

يحصل ويضبط قيمة النطاق.

```csharp
public object Value { get; set; }
```

### ملاحظات

إذا كان النطاق يحتوي على عدة خلايا، يجب أن يكون الكائن المرتجع/المطبق مصفوفة ذات بعدين

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق يبدأ من A1 ويغطي 3×3 خلايا
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");

            // ضبط مصفوفة ثنائية الأبعاد كقيمة للنطاق
            int[,] values = new int[3, 3] { { 1, 2, 3 }, { 4, 5, 6 }, { 7, 8, 9 } };
            range.Value = values;

            // احفظ المصنف
            workbook.Save("RangePropertyValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


