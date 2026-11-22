---
title: "الفئة AbstractCalculationMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.AbstractCalculationMonitor. مراقب للمستخدم لتتبع تقدم حساب الصيغة"
type: docs
url: /ar/net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

مراقبة للمستخدم لتتبع تقدم حساب الصيغة.

```csharp
public abstract class AbstractCalculationMonitor
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue/) { get; } | يحصل على القيمة المحسوبة حديثًا للخلية. يجب استخدامه فقط في [`AfterCalculate`](./aftercalculate/). |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue/) { get; } | يحصل على القيمة القديمة للخلية المحسوبة. يجب استخدامه فقط في [`BeforeCalculate`](./beforecalculate/) و[`AfterCalculate`](./aftercalculate/). |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged/) { get; } | ما إذا تم تغيير قيمة الخلية بعد الحساب. يجب استخدامه فقط في [`AfterCalculate`](./aftercalculate/). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate/)(int, int, int) | نفّذ هذه الطريقة للقيام بالمعالجة بعد حساب خلية واحدة. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate/)(int, int, int) | نفّذ هذه الطريقة للقيام بالمعالجة قبل حساب خلية واحدة. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular/)(IEnumerator) | نفّذ هذه الطريقة للقيام بالأعمال عند حساب الصيغ ذات المراجع الدائرية. |

### أمثلة

```csharp
using Aspose.Cells;
using System;
using System.Collections;

namespace AsposeCellsExamples
{
    // تنفيذ مخصص لـ AbstractCalculationMonitor
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"Before calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"After calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
            Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
        }

        public override bool OnCircular(IEnumerator circularCellsData)
        {
            Console.WriteLine("Circular reference detected.");
            return false; // Return false to stop calculation when circular reference is detected
        }
    }

    public class CalculationMonitorDemo
    {
        public static void RunDemo()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // أنشئ مثيلاً من CustomCalculationMonitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();

            // عيّن خيارات الحساب
            CalculationOptions options = new CalculationOptions
            {
                CalculationMonitor = monitor,
                IgnoreError = false,
                Recursive = true
            };

            // احسب الصيغ باستخدام المراقب المخصص
            workbook.CalculateFormula(options);

            // احفظ المصنف
            workbook.Save("CalculationMonitorDemo.xlsx");
            workbook.Save("CalculationMonitorDemo.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


