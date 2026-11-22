---
title: "CalculationData.CellColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationData. تحصل على فهرس العمود للخلية التي توجد فيها الدالة"
type: docs
url: /ar/net/aspose.cells/calculationdata/cellcolumn/
---
## CalculationData.CellColumn property

يحصل على فهرس العمود للخلية التي توجد فيها الدالة.

```csharp
public int CellColumn { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellColumnDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف بيانات عينة مع صيغ في أعمدة مختلفة
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["B1"].PutValue(20);
                worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

                // إنشاء خيارات الحساب باستخدام محرك مخصص
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellColumnDemoEngine();

                // حساب الصيغ
                workbook.CalculateFormula(options);

                // اعرض النتيجة المحسوبة
                Console.WriteLine("Calculated value in C1: " + worksheet.Cells["C1"].Value);

                // حفظ النتيجة
                workbook.Save("CellColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellColumnDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data != null)
            {
                // الوصول إلى خاصية CellColumn للقراءة فقط
                int columnIndex = data.CellColumn;
                Console.WriteLine($"Function is in column index: {columnIndex}");

                // عرض استخدام معلومات العمود
                if (data.FunctionName == "SUM")
                {
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
}
```

### انظر أيضًا

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


