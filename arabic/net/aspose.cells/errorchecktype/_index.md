---
title: "التعداد ErrorCheckType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.ErrorCheckType. يمثل جميع أنواع فحص الأخطاء"
type: docs
url: /ar/net/aspose.cells/errorchecktype/
---
## ErrorCheckType enumeration

يمثل جميع أنواع فحص الأخطاء.

```csharp
public enum ErrorCheckType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| EvaluationError | `1` | تجاهل الأخطاء عندما تحتوي الخلايا على صيغ تؤدي إلى خطأ. |
| Calc | `1` |  |
| EmptyCellRef | `2` | تجاهل الأخطاء عندما تشير الصيغ إلى خلايا فارغة. |
| NumberStoredAsText | `4` | تجاهل الأخطاء عندما تكون الأرقام مُنسقة كنص أو يسبقها علامة اقتباس مفردة |
| TextNumber | `4` | تجاهل الأخطاء عندما تكون الأرقام مُنسقة كنص أو يسبقها علامة اقتباس مفردة |
| InconsistRange | `8` | تجاهل الأخطاء عندما تُغفل الصيغ عن خلايا معينة في منطقة. |
| InconsistFormula | `16` | تجاهل الأخطاء عندما تختلف صيغة في منطقة من ورقة العمل الخاصة بك عن صيغ أخرى في نفس المنطقة. |
| TwoDigitTextYear | `32` | تجاهل الأخطاء عندما تحتوي الصيغ على خلايا مُنسقة كنص مع سنوات ممثلة برقمين. |
| TextDate | `32` | تجاهل الأخطاء عندما تحتوي الصيغ على خلايا مُنسقة كنص مع سنوات ممثلة برقمين. |
| UnlockedFormula | `64` | تجاهل الأخطاء عندما تحتوي الخلايا غير المقفلة على صيغ. |
| UnproctedFormula | `64` | تجاهل الأخطاء عندما تحتوي الخلايا غير المقفلة على صيغ. |
| TableDataValidation | `128` | تجاهل الأخطاء عندما لا يتوافق قيمة خلية في جدول مع قواعد التحقق من صحة البيانات المحددة. |
| Validation | `128` | تجاهل الأخطاء عندما لا يتوافق قيمة خلية في جدول مع قواعد التحقق من صحة البيانات المحددة. |
| CalculatedColumn | `129` | تجاهل الأخطاء عندما تحتوي الخلايا على قيمة تختلف عن صيغة العمود المحسوبة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckTypeDemo
    {
        public static void ErrorCheckTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى ErrorCheckOptionCollection
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // إضافة ErrorCheckOption جديد
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];

            // تعيين أنواع فحص الأخطاء المختلفة إلى false
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.Validation, false);

            // تحديد منطقة خلية لخيار فحص الأخطاء
            CellArea cellArea = CellArea.CreateCellArea("A1", "B10");
            errorCheckOption.AddRange(cellArea);

            // احفظ المصنف
            workbook.Save("ErrorCheckTypeExample.xlsx");
            workbook.Save("ErrorCheckTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


