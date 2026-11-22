---
title: "Validation.AddAreas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Validation. تطبق التحقق على المناطق المحددة"
type: docs
url: /ar/net/aspose.cells/validation/addareas/
---
## Validation.AddAreas method

يطبق التحقق على المناطق المحددة.

```csharp
public void AddAreas(CellArea[] areas, bool checkIntersection, bool checkEdge)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المناطق | CellArea[] | المناطق. |
| checkIntersection | منطقي | ما إذا تم التحقق من تقاطع المنطقة المحددة مع مناطق التحقق الحالية. إذا تم تطبيق تحقق واحد في المنطقة المحددة (أو جزء منها)، يجب إزالة التحقق الحالي أولاً من المنطقة المحددة. وإلا قد يحدث تلف في عمليات التحقق المُولَّدة. إذا كان المستخدم متأكدًا من أن جميع المناطق المضافة لا تتقاطع مع أي منطقة موجودة، يمكن ضبط هذا المعامل على false لأسباب تتعلق بالأداء. |
| checkEdge | منطقي | ما إذا تم التحقق من حافة المناطق التي تم تطبيق هذا التحقق عليها. تعتمد الإعدادات الداخلية للتحقق على أعلى اليسار من نطاقاته المطبقة، لذلك إذا أصبحت إحدى المناطق المحددة هي أعلى اليسار الجديدة للنطاقات المطبقة، يجب تغيير وإعادة بناء الإعدادات الداخلية، وإلا قد يحدث نتيجة غير متوقعة. إذا كان المستخدم متأكدًا من أن أيًا من تلك المناطق المضافة ليست أعلى اليسار، يمكن ضبط هذا المعامل على false لأسباب تتعلق بالأداء. |

### ملاحظات

في هذه الطريقة، سنقوم بإزالة جميع عمليات التحقق القديمة في المنطقة المعطاة. بالنسبة لأعلى منطقة يسار من نطاقات Validation المطبقة، أولاً يكون StartRow هو الأصغر، ثانياً يكون StartColumn هو الأصغر بين تلك المناطق التي لها نفس أصغر StartRow.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodAddAreasWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.List;
            validation.AlertStyle = ValidationAlertType.Stop;
            validation.Operator = OperatorType.None;
            validation.Formula1 = "1,2,3";
            validation.InCellDropDown = true;

            CellArea[] areas = new CellArea[2];
            areas[0] = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 1 };
            areas[1] = new CellArea { StartRow = 2, StartColumn = 2, EndRow = 3, EndColumn = 3 };

            try
            {
                validation.AddAreas(areas, true, false);
                Console.WriteLine("Added validation areas with checkIntersection=true, checkEdge=false");

                foreach (CellArea area in validation.Areas)
                {
                    Console.WriteLine($"Validation area: R{area.StartRow + 1}C{area.StartColumn + 1}:R{area.EndRow + 1}C{area.EndColumn + 1}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding validation areas: {ex.Message}");
            }

            workbook.Save("ValidationAddAreasDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


