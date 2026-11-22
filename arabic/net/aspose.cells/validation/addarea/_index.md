---
title: "Validation.AddArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Validation. تطبق التحقق على المنطقة"
type: docs
url: /ar/net/aspose.cells/validation/addarea/
---
## AddArea(CellArea) {#addarea}

يطبق التحقق على المنطقة.

```csharp
public void AddArea(CellArea cellArea)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | CellArea | المنطقة. |

### ملاحظات

إنه يعادل استخدام `AddArea` مع فحص التقاطع والحافة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // إنشاء تحقق
            ValidationCollection vc = sheet.Validations;
            Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
            validation.Type = ValidationType.List;
            validation.Formula1 = "=A1:A10";

            // إضافة المزيد من المناطق إلى التحقق
            for (int i = 1; i < 5; i++)
            {
                validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
            }

            // احفظ المصنف
            wb.Save("ValidationMethodAddAreaWithCellAreaDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Validation with multiple areas created successfully.");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddArea(CellArea, bool, bool) {#addarea_1}

يطبق التحقق على المنطقة.

```csharp
public void AddArea(CellArea cellArea, bool checkIntersection, bool checkEdge)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | CellArea | المنطقة. |
| checkIntersection | منطقي | ما إذا كان يتم فحص تقاطع المنطقة المعطاة مع مناطق عمليات التحقق الموجودة. إذا تم تطبيق عملية تحقق في المنطقة المعطاة (أو جزء منها)، يجب إزالة عملية التحقق الموجودة أولاً من المنطقة المعطاة. وإلا قد يحدث تلف في عمليات التحقق المولدة. إذا كان المستخدم متأكدًا من أن المنطقة المضافة لا تتقاطع مع أي منطقة موجودة، يمكن ضبط هذا المعامل كقيمة false لأغراض الأداء. |
| checkEdge | منطقي | ما إذا كان يتم فحص حافة المناطق التي تم تطبيق هذا التحقق عليها. تعتمد الإعدادات الداخلية للـ Validation على أعلى منطقة يسار من نطاقاته المطبقة، لذا إذا أصبحت المنطقة المعطاة هي أعلى منطقة يسار جديدة للنطاقات المطبقة، يجب تغيير وإعادة بناء الإعدادات الداخلية، وإلا قد يحدث نتيجة غير متوقعة. إذا كان المستخدم متأكدًا من أن المنطقة المضافة ليست أعلى منطقة يسار، يمكن ضبط هذا المعامل كقيمة false لأغراض الأداء. |

### ملاحظات

في هذه الطريقة، سنقوم بإزالة جميع عمليات التحقق القديمة في المنطقة المعطاة. بالنسبة لأعلى منطقة يسار من نطاقات Validation المطبقة، أولاً يكون StartRow هو الأصغر، ثانياً يكون StartColumn هو الأصغر بين تلك المناطق التي لها نفس أصغر StartRow.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل والحصول على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء تحقق في منطقة محددة
            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "F3";

            // توضيح AddArea باستخدام CellArea ومعاملين منطقين
            validation.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
            Console.WriteLine("Area count after AddArea: " + validation.Areas.Length);
            Console.WriteLine("Formula1 after AddArea: " + validation.Formula1);

            // إزالة المنطقة المضافة
            validation.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
            Console.WriteLine("Area count after RemoveArea: " + validation.Areas.Length);

            // إضافة مناطق متعددة باستخدام عملية جماعية
            CellArea[] areas = new CellArea[10];
            for (int i = 0; i < areas.Length; i++)
            {
                areas[i] = CellArea.CreateCellArea(6 + i, 3, 6 + i, 4);
            }
            validation.AddAreas(areas, true, true);
            Console.WriteLine("Area count after bulk AddAreas: " + validation.Areas.Length);

            // احفظ المصنف
            workbook.Save("ValidationMethodAddAreaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


