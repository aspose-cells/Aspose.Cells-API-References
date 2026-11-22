---
title: "CalculationData.Workbook"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationData. تحصل على كائن Workbook حيث تكون الدالة"
type: docs
url: /ar/net/aspose.cells/calculationdata/workbook/
---
## CalculationData.Workbook property

يحصل على كائن Workbook حيث توجد الدالة.

```csharp
public Workbook Workbook { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorkbookDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية وصيغة
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].Formula = "=CUSTOMFUNC()";

            // إنشاء خيارات الحساب وتسجيل محرك حساب مخصص
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();

            // تشغيل الحساب باستخدام الخيارات لعرض استخدام خاصية Workbook
            workbook.CalculateFormula(options);

            // عرض النتيجة من الحساب
            Console.WriteLine("Calculated value in B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("Modified value in C1: " + worksheet.Cells["C1"].Value);

            // حفظ النتيجة
            workbook.Save("PropertyWorkbookDemo.xlsx");
        }

        private class CustomCalcEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "CUSTOMFUNC")
                {
                    // الوصول إلى خاصية Workbook من CalculationData
                    Workbook currentWorkbook = data.Workbook;
                    Worksheet currentSheet = currentWorkbook.Worksheets[0];

                    // عرض كيفية استخدام workbook لتعديل البيانات
                    double inputValue = (double)currentSheet.Cells["A1"].Value;
                    currentSheet.Cells["C1"].PutValue(inputValue * 2);

                    // تعيين النتيجة المحسوبة
                    data.CalculatedValue = inputValue * 3;
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../../workbook/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


