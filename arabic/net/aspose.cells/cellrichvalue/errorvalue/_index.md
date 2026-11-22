---
title: "CellRichValue.ErrorValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellRichValue. يحصل على نوع قيمة الخطأ للخلية"
type: docs
url: /ar/net/aspose.cells/cellrichvalue/errorvalue/
---
## CellRichValue.ErrorValue property

يحصل على نوع قيمة الخطأ للخلية.

```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyErrorValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أنشئ خطأ تسرب في الخلية A1
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3})";
            
            try
            {
                // احسب الصيغ لتوليد خطأ التسرب
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // خطأ تسرب متوقع.
            }
            
            // احصل على القيمة الغنية من الخلية A1
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // تحقق واعرض نوع الخطأ
            Console.WriteLine("Error type: " + richValue.ErrorValue);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


