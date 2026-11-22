---
title: "Worksheet.Validations"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل على مجموعة إعدادات التحقق من البيانات في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

يحصل على مجموعة إعدادات التحقق من صحة البيانات في ورقة العمل.

```csharp
public ValidationCollection Validations { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyValidationsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف التحقق من البيانات إلى الخلية A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // تصحيح: إنشاء CellArea مع StartRow و StartColumn و EndRow و EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // احصل على التحقق من البيانات من الخلية A1
            Validation cellValidation = worksheet.Validations.GetValidationInCell(0, 0);
            
            // إخراج نوع التحقق
            Console.WriteLine("Validation type in A1: " + cellValidation.Type);
            
            // احفظ المصنف
            workbook.Save("ValidationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


