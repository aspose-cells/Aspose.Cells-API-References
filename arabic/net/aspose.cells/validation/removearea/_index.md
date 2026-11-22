---
title: "Validation.RemoveArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Validation. إزالة إعدادات التحقق في النطاق"
type: docs
url: /ar/net/aspose.cells/validation/removearea/
---
## Validation.RemoveArea method

إزالة إعدادات التحقق في النطاق.

```csharp
public void RemoveArea(CellArea cellArea)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | CellArea | المناطق التي يجب إزالة إعدادات التحقق منها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تحققًا إلى ورقة العمل
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // إضافة منطقة التحقق الأولية
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            validation.AddArea(initialArea);

            // إضافة منطقة أخرى إلى التحقق
            CellArea additionalArea = CellArea.CreateCellArea(1, 1, 1, 1);
            validation.AddArea(additionalArea);

            Console.WriteLine("Validation areas count after adding: " + validation.Areas.Length);

            // إزالة المنطقة الإضافية
            validation.RemoveArea(additionalArea);

            Console.WriteLine("Validation areas count after removing: " + validation.Areas.Length);

            // إضافة مناطق متعددة
            CellArea[] multipleAreas = new CellArea[]
            {
                CellArea.CreateCellArea(2, 2, 2, 2),
                CellArea.CreateCellArea(3, 3, 3, 3),
                CellArea.CreateCellArea(4, 4, 4, 4)
            };
            validation.AddAreas(multipleAreas, false, false);

            Console.WriteLine("Validation areas count after adding multiple: " + validation.Areas.Length);

            // إزالة إحدى المناطق
            validation.RemoveArea(multipleAreas[1]);

            Console.WriteLine("Validation areas count after removing one: " + validation.Areas.Length);
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


