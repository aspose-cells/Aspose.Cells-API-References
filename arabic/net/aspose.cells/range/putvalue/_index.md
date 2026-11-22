---
title: "Range.PutValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تضع قيمة في النطاق إذا كان ذلك مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق أرقام الخلايا"
type: docs
url: /ar/net/aspose.cells/range/putvalue/
---
## Range.PutValue method

يضع قيمة في النطاق، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الرقم للخلية.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | String | قيمة الإدخال |
| isConverted | منطقي | صحيح: تم تحويله إلى نوع بيانات آخر إذا كان مناسبًا. |
| setStyle | منطقي | صحيح: تعيين تنسيق الرقم إلى نمط الخلية عند التحويل إلى نوع بيانات آخر |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1:B10");
            range.PutValue("123", true, false);
            
            Console.WriteLine("Value at A5: " + cells["A5"].DoubleValue);
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


