---
title: "CalculationOptions.CalculationMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationOptions. المراقب للمستخدم لتتبع تقدم حساب الصيغة"
type: docs
url: /ar/net/aspose.cells/calculationoptions/calculationmonitor/
---
## CalculationOptions.CalculationMonitor property

المراقب للمستخدم لتتبع تقدم حساب الصيغ.

```csharp
public AbstractCalculationMonitor CalculationMonitor { get; set; }
```

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalculationMonitorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بعض الصيغ النموذجية
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // إنشاء خيارات حساب مع مراقب مخصص
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new SampleCalculationMonitor();

            // حساب الصيغ مع المراقبة
            workbook.CalculateFormula(options);

            // إخراج النتائج
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("A2: " + worksheet.Cells["A2"].Value);
            Console.WriteLine("A3: " + worksheet.Cells["A3"].Value);
        }
    }

    public class SampleCalculationMonitor : AbstractCalculationMonitor
    {
        public override bool OnCircular(IEnumerator circularCellsData)
        {
            // معالجة المراجع الدائرية إذا لزم الأمر
            return base.OnCircular(circularCellsData);
        }

        public override void BeforeCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Before calculation: Sheet{sheetIndex}, Row{rowIndex}, Col{columnIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"After calculation: Sheet{sheetIndex}, Row{rowIndex}, Col{columnIndex}");
        }
    }
}
```

### انظر أيضًا

* class [AbstractCalculationMonitor](../../abstractcalculationmonitor/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


