---
title: "CalculationData.Worksheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationData. يحصل على كائن Worksheet حيث توجد الدالة"
type: docs
url: /ar/net/aspose.cells/calculationdata/worksheet/
---
## CalculationData.Worksheet property

يحصل على كائن Worksheet حيث توجد الدالة.

```csharp
public Worksheet Worksheet { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorksheetDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // إضافة بعض البيانات لجعل المثال ذو معنى
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // إنشاء خيارات الحساب باستخدام محرك مخصص
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new WorksheetDemoEngine();

                // حساب الصيغ مع خيارات
                workbook.CalculateFormula(options);

                // اعرض النتيجة
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // حفظ النتيجة
                workbook.Save("WorksheetDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class WorksheetDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // الوصول إلى خاصية Worksheet للقراءة فقط
                Worksheet worksheet = data.Worksheet;
                Console.WriteLine($"Function is in worksheet: {worksheet.Name}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


