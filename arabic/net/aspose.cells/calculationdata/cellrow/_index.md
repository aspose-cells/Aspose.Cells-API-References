---
title: "CalculationData.CellRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationData. يحصل على فهرس الصف للخلية التي توجد فيها الدالة"
type: docs
url: /ar/net/aspose.cells/calculationdata/cellrow/
---
## CalculationData.CellRow property

يحصل على فهرس الصف للخلية التي توجد فيها الدالة.

```csharp
public int CellRow { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCellRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // قم بتعيين بعض البيانات النموذجية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // عيّن خيارات الحساب
            CalculationOptions opts = new CalculationOptions();
            opts.CustomEngine = new CustomCalculationEngine();

            // حساب الصيغ
            workbook.CalculateFormula(opts);

            // الوصول إلى الخلية المحسوبة وإظهار خاصية CellRow
            Cell calculatedCell = worksheet.Cells["A3"];
            Console.WriteLine("Calculated cell is at row: " + calculatedCell.Row);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // عرض كيفية الوصول إلى معلومات الصف من بيانات الحساب
            if (data != null)
            {
                Console.WriteLine("Current calculation is for row: " + data.CellRow);
            }
        }
    }
}
```

### انظر أيضًا

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


