---
title: "الفئة ErrorCheckOption"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ErrorCheckOption. إعداد فحص الأخطاء المطبق على نطاقات معينة"
type: docs
url: /ar/net/aspose.cells/errorcheckoption/
---
## ErrorCheckOption class

إعداد فحص الأخطاء المطبق على نطاقات معينة.

```csharp
public class ErrorCheckOption
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddRange](../../aspose.cells/errorcheckoption/addrange/)(CellArea) | يضيف نطاقًا واحدًا متأثرًا بهذا الإعداد. |
| [GetCountOfRange](../../aspose.cells/errorcheckoption/getcountofrange/)() | يحصل على عدد النطاقات المتأثرة بهذا الإعداد. |
| [GetRange](../../aspose.cells/errorcheckoption/getrange/)(int) | يحصل على النطاق المتأثر بهذا الإعداد وفق الفهرس المعطى. |
| [IsErrorCheck](../../aspose.cells/errorcheckoption/iserrorcheck/)(ErrorCheckType) | يتحقق مما إذا كان نوع الخطأ المعطى سيُفحص. |
| [RemoveRange](../../aspose.cells/errorcheckoption/removerange/)(int) | يزيل نطاقًا واحدًا وفق الفهرس المعطى. |
| [SetErrorCheck](../../aspose.cells/errorcheckoption/seterrorcheck/)(ErrorCheckType, bool) | يضبط ما إذا كان نوع الخطأ المعطى سيُفحص. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionDemo
    {
        public static void ErrorCheckOptionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على ErrorCheckOptionCollection من ورقة العمل
            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;

            // أضف ErrorCheckOption جديد إلى المجموعة
            int optionIdx = opts.Add();
            ErrorCheckOption opt = opts[optionIdx];

            // تعيين خيارات فحص الأخطاء
            opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(ErrorCheckType.TextDate, false);
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.SetErrorCheck(ErrorCheckType.Validation, false);

            // حدد نطاق خلية وأضفه إلى ErrorCheckOption
            CellArea ca = CellArea.CreateCellArea("A1", "B10");
            opt.AddRange(ca);

            // احفظ المصنف
            workbook.Save("ErrorCheckOptionExample.xlsx");
            workbook.Save("ErrorCheckOptionExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


