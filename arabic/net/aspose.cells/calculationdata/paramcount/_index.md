---
title: "CalculationData.ParamCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationData. تحصل على عدد المعاملات"
type: docs
url: /ar/net/aspose.cells/calculationdata/paramcount/
---
## CalculationData.ParamCount property

يحصل على عدد المعلمات

```csharp
public int ParamCount { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyParamCountDemo
    {
        public static void Run()
        {
            try
            {
                // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // ملء بعض الخلايا التي ستُستخدم كمعاملات
                sheet.Cells["A1"].PutValue(10);
                sheet.Cells["A2"].PutValue(20);
                sheet.Cells["A3"].PutValue(30);

                // تعيين صيغة تستدعي دالة مخصصة مع ثلاثة معاملات
                sheet.Cells["B1"].Formula = "=DEMOPARAM(A1, A2, A3)";

                // تكوين خيارات الحساب لاستخدام محرك مخصص
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ParamCountEngine();

                // إجراء حساب
                workbook.CalculateFormula(options);

                // المحرك المخصص يُعيد ParamCount كالقيمة المحسوبة
                Console.WriteLine("ParamCount reported by custom function: " + sheet.Cells["B1"].Value);
                
                // احفظ المصنف اختياريًا
                workbook.Save("ParamCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // محرك حساب مخصص يُظهر قراءة خاصية ParamCount
        private class ParamCountEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // حدد الدالة المخصصة بالاسم
                if (data.FunctionName != null && data.FunctionName.Equals("DEMOPARAM", StringComparison.OrdinalIgnoreCase))
                {
                    // قراءة خاصية ParamCount للقراءة فقط
                    int count = data.ParamCount;

                    // استخدم العد كنتيجة للدالة
                    data.CalculatedValue = count;
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


