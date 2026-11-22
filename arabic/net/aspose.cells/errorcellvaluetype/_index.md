---
title: "التعداد ErrorCellValueType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.ErrorCellValueType. يمثل قيمة خلية تحتوي على خطأ"
type: docs
url: /ar/net/aspose.cells/errorcellvaluetype/
---
## ErrorCellValueType enumeration

يمثل قيمة خلية تحتوي على خطأ.

```csharp
public enum ErrorCellValueType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Value | `1` | يمثل قيمة خلية تحتوي على خطأ #VALUE!. |
| Ref | `3` | يمثل قيمة خلية تحتوي على خطأ #REF!. |
| Name | `4` | يمثل قيمة خلية تحتوي على خطأ #NAME?. |
| NA | `6` | يمثل قيمة خلية تحتوي على خطأ #N/A. |
| Blocked | `10` | يمثل قيمة خلية تحتوي على خطأ #BLOCKED!. |
| Busy | `14` | يمثل قيمة خلية تحتوي على خطأ #BUSY!. |
| Calc | `13` | يمثل قيمة خلية تحتوي على خطأ #CALC!. |
| Connect | `9` | يمثل قيمة خلية تحتوي على خطأ #CONNECT!. |
| Field | `12` | يمثل قيمة خلية تحتوي على خطأ #FIELD!. |
| Spill | `8` | يمثل قيمة خلية تحتوي على خطأ #SPILL!. |
| Unknown | `11` | يمثل قيمة خلية تحتوي على خطأ #UNKNOWN!. |
| TimeOut | `19` | يمثل قيمة خلية تحتوي على خطأ #TIMEOUT!. |
| External | `18` | يمثل قيمة خلية تحتوي على خطأ #EXTERNAL!. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassErrorCellValueTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بتعيين صيغة ستؤدي إلى خطأ تسرب.
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3;1,2,3})";
            
            try
            {
                // احسب الصيغ لتفعيل الخطأ.
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // خطأ تسرب متوقع.
            }
            
            // احصل على القيمة الغنية للخلية.
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // تحقق من نوع الخطأ.
            if (richValue.ErrorValue == ErrorCellValueType.Spill)
            {
                Console.WriteLine("Cell contains a spill error as expected");
            }
            
            // احفظ المصنف
            workbook.Save("ErrorCellValueTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


