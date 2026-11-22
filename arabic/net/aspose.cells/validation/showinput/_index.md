---
title: "Validation.ShowInput"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Validation. تشير إلى ما إذا كانت رسالة إدخال التحقق من البيانات ستظهر كلما اختار المستخدم خلية في نطاق التحقق"
type: docs
url: /ar/net/aspose.cells/validation/showinput/
---
## Validation.ShowInput property

يشير إلى ما إذا كانت رسالة إدخال التحقق من البيانات ستُعرض كلما اختار المستخدم خلية في نطاق التحقق من البيانات.

```csharp
public bool ShowInput { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowInputDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء منطقة تحقق
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;

            // إضافة تحقق
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // تعيين خاصية ShowInput
            validation.ShowInput = true;
            validation.InputTitle = "Selection";
            validation.InputMessage = "Please select Yes or No";

            validation.AddArea(area);

            // احفظ المصنف
            workbook.Save("ValidationPropertyShowInputDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


