---
title: "CellsHelper.ConvertA1FormulaToR1C1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. تحول صيغة A1 للخلية إلى صيغة r1c1"
type: docs
url: /ar/net/aspose.cells/cellshelper/converta1formulator1c1/
---
## CellsHelper.ConvertA1FormulaToR1C1 method

تحول صيغة A1 للخلية إلى صيغة r1c1.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertA1FormulaToR1C1(string formula, int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | معادلة A1. |
| صف | Int32 | فهرس الصف للخلية. |
| عمود | Int32 | فهرس العمود للخلية. |

### قيمة الإرجاع

صيغة R1C1.

### ملاحظات

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة Worksheet.ConvertFormulaReferenceStyle(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertA1FormulaToR1C1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // تحويل صيغة النمط A1 إلى نمط R1C1
            string r1c1Formula = CellsHelper.ConvertA1FormulaToR1C1("=A1+B2", 0, 0);
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


