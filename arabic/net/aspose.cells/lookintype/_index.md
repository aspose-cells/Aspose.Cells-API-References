---
title: "تعداد LookInType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.LookInType. يمثل نوع البحث"
type: docs
url: /ar/net/aspose.cells/lookintype/
---
## LookInType enumeration

يمثل نوع البحث داخل.

```csharp
public enum LookInType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Formulas | `0` | يبحث عن الكائن المطلوب من الصيغة([`Formula`](../cell/formula/)) إذا كانت الخلية صيغة، وإلا يبحث من القيمة الأصلية للخلية (نفس OriginalValues). |
| Values | `1` | يبحث عن الكائن من القيمة الأصلية للخلية([`Value`](../cell/value/)) والقيمة المُنسقة([`StringValue`](../cell/stringvalue/)). |
| ValuesExcludeFormulaCell | `2` | يتجاهل الخلايا التي هي صيغ. بالنسبة للخلايا التي ليست صيغًا، يكون الأمر مماثلًا للقيم. |
| Comments | `3` | يبحث عن الكائن من تعليق الخلية فقط. يتجاهل الخلايا التي لا تحتوي على تعليق. |
| OnlyFormulas | `4` | يتجاهل الخلايا التي ليست صيغًا. بالنسبة للخلايا التي هي صيغ، يبحث عن الكائن المطلوب من الصيغة([`Formula`](../cell/formula/)). |
| OriginalValues | `5` | ابحث عن الكائن من القيمة الأصلية للخلية فقط. |
| FormattedValues | `6` | ابحث عن الكائن من القيمة المُنسقة للخلية([`StringValue`](../cell/stringvalue/)) فقط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassLookInTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات والصيغ
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].Formula = "=A1";
            worksheet.Cells["C1"].PutValue("Contains B1");

            // ابحث عن الخلية التي تحتوي على صيغة مع "B1"
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            Cell foundCell = worksheet.Cells.Find("B1", null, options);

            // أخرج النتيجة.
            if (foundCell != null)
            {
                Console.WriteLine($"Found cell at row: {foundCell.Row}, column: {foundCell.Column}");
                Console.WriteLine($"Cell value: {foundCell.StringValue}");
                Console.WriteLine($"Cell formula: {foundCell.Formula}");
            }
            else
            {
                Console.WriteLine("Cell not found");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


