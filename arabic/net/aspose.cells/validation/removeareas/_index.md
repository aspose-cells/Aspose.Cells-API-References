---
title: "Validation.RemoveAreas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Validation. تزيل هذا التحقق من المناطق المحددة"
type: docs
url: /ar/net/aspose.cells/validation/removeareas/
---
## Validation.RemoveAreas method

يزيل هذا التحقق من المناطق المحددة.

```csharp
public void RemoveAreas(CellArea[] areas)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المناطق | CellArea[] | المناطق التي يجب إزالة إعدادات التحقق منها. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodRemoveAreasWithCellAreaArrayDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تحقق من البيانات إلى ورقة العمل
            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            
            // تكوين إعدادات التحقق
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "10";

            // إنشاء منطقتين من الخلايا للتحقق
            CellArea area1 = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 1,
                EndColumn = 1
            };  // A1:B2
            CellArea area2 = new CellArea
            {
                StartRow = 2,
                StartColumn = 2,
                EndRow = 3,  // Original code had (2,2,1,1) which would be invalid endRow < startRow
                EndColumn = 3
            };  // C3:D4 (corrected end coordinates)
            
            // إضافة المناطق إلى التحقق
            validation.AddArea(area1);
            validation.AddArea(area2);
            Console.WriteLine($"Added areas: {validation.Areas.Length}");

            try
            {
                // إنشاء مصفوفة بمنطقة واحدة للإزالة
                CellArea[] removeAreas = { area1 };
                
                // تنفيذ طريقة RemoveAreas
                validation.RemoveAreas(removeAreas);
                Console.WriteLine($"Remaining areas after removal: {validation.Areas.Length}");
                
                // عرض إحداثيات المناطق المتبقية
                foreach (CellArea remainingArea in validation.Areas)
                {
                    Console.WriteLine($"Area: {remainingArea.StartRow},{remainingArea.StartColumn} to {remainingArea.EndRow},{remainingArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // حفظ المصنف المعدل
            workbook.Save("ValidationRemoveAreasDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


