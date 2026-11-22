---
title: "Validation.Operator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Validation. تمثل العامل لعملية التحقق من البيانات"
type: docs
url: /ar/net/aspose.cells/validation/operator/
---
## Validation.Operator property

يمثل العامل للتحقق من البيانات.

```csharp
public OperatorType Operator { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyOperatorDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للتحقق
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // إنشاء نطاق تحقق
            CellArea area = CellArea.CreateCellArea("B1", "B5");
            int validationIndex = worksheet.Validations.Add(area);
            Validation validation = worksheet.Validations[validationIndex];

            // تعيين خصائص التحقق مع توضيح Operator
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "30";
            validation.ShowError = true;
            validation.ErrorMessage = "Value must be between 10 and 30";

            // احفظ المصنف
            workbook.Save("ValidationOperatorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


