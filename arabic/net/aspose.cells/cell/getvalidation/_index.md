---
title: "Cell.GetValidation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحصل على التحقق المطبق على هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

يحصل على التحقق من الصحة المطبق على هذه الخلية.

```csharp
public Validation GetValidation()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية B5 وإضافة التحقق
            Cell cell = worksheet.Cells["B5"];
            Validation validation = cell.GetValidation();
            
            // تعيين نوع التحقق وعرض الرسالة
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            validation.ShowError = true;
            validation.ErrorMessage = "Enter value between 10 and 20";
            
            // احفظ المصنف
            workbook.Save("ValidationDemo.xlsx");
            
            // التحقق من صحة التحقق
            Validation retrievedValidation = cell.GetValidation();
            Console.WriteLine("Validation Type: " + retrievedValidation.Type);
            Console.WriteLine("Validation Message: " + retrievedValidation.ErrorMessage);
        }
    }
}
```

### انظر أيضًا

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


