---
title: "CalculationOptions.CustomEngine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationOptions. محرك حساب الصيغ المخصص لتوسيع محرك الحساب الافتراضي في Aspose.Cells"
type: docs
url: /ar/net/aspose.cells/calculationoptions/customengine/
---
## CalculationOptions.CustomEngine property

محرك حساب الصيغ المخصص لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

```csharp
public AbstractCalculationEngine CustomEngine { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCustomEngineDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // تعيين صيغة HYPERLINK في الخلية A1
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://example.com\",\"Click Here\")";
            
            // إنشاء محرك مخصص يعالج دالة HYPERLINK
            CustomEngineForHyperlink customEngine = new CustomEngineForHyperlink(true);
            
            // تعيين خيارات الحساب مع محرك مخصص
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = customEngine;
            
            // احسب الصيغ باستخدام المحرك المخصص
            wb.CalculateFormula(options);
            
            Console.WriteLine("Custom engine invoked: " + customEngine.Invoked);
        }
    }

    public class CustomEngineForHyperlink : AbstractCalculationEngine
    {
        public bool Invoked { get; private set; }
        private readonly bool _shouldProcess;

        public CustomEngineForHyperlink(bool shouldProcess)
        {
            _shouldProcess = shouldProcess;
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "HYPERLINK" && _shouldProcess)
            {
                Invoked = true;
                data.CalculatedValue = "[Custom Processed] " + data.GetParamText(1);
            }
            // لا تستدعي base.Calculate() لأنه مجرد
            // فقط دع الحساب الافتراضي يحدث للوظائف الأخرى
        }
    }
}
```

### انظر أيضًا

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


