---
title: "Validation.InputTitle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Validation. تمثل عنوان مربع حوار إدخال التحقق من البيانات"
type: docs
url: /ar/net/aspose.cells/validation/inputtitle/
---
## Validation.InputTitle property

يمثل عنوان مربع حوار إدخال التحقق من البيانات.

```csharp
public string InputTitle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputTitleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن تحقق
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.IgnoreBlank = true;
            
            // تعيين نطاق التحقق
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // تعيين خصائص التحقق
            validation.Formula1 = "10";
            validation.Formula2 = "100";
            validation.Operator = OperatorType.Between;
            
            // تعيين خصائص رسالة الإدخال
            validation.InputTitle = "Number Validation";
            validation.InputMessage = "Please enter a number between 10 and 100";
            
            // احفظ المصنف
            workbook.Save("ValidationInputTitleDemo.xlsx");
            
            // تحقق من خاصية InputTitle
            Console.WriteLine("Validation InputTitle: " + validation.InputTitle);
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


