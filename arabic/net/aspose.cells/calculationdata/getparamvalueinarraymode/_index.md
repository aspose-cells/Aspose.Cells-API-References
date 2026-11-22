---
title: "CalculationData.GetParamValueInArrayMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CalculationData. تحصل على قيم المعامل عند فهرس محدد. إذا كان المعامل نوعًا من التعبير يحتاج إلى حساب، فسيتم حسابه في وضع المصفوفة"
type: docs
url: /ar/net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

يحصل على القيمة (القيم) للمعامل عند فهرس معين. إذا كان المعامل نوعًا من التعبير يحتاج إلى حساب، فسيتم حسابه في وضع المصفوفة.

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس المعامل (بدءًا من 0) |
| maxRowCount | Int32 | حد عدد الصفوف للمصفوفة المرجعة. إذا كان غير إيجابي أو أكبر من عدد الصفوف الفعلي، فسيُستخدم عدد الصفوف الفعلي. |
| maxColumnCount | Int32 | حد عدد الأعمدة للمصفوفة المرجعة. إذا كان غير إيجابي أو أكبر من عدد الصفوف الفعلي، فسيُستخدم عدد الأعمدة الفعلي. |

### قيمة الإرجاع

مصفوفة تحتوي على جميع العناصر التي يمثلها المعامل المحدد.

### ملاحظات

لتعبير يحتاج إلى حساب، مع أخذ A:A+B:B كمثال: في وضع القيمة سيتم حسابه إلى قيمة واحدة وفقًا لقاعدة الخلية الحالية. ولكن في وضع المصفوفة، سيتم حساب جميع قيم A1+B1،A2+B2،A3+B3،... واستخدامها لإنشاء المصفوفة المرجعة. وفي مثل هذه الحالة، من الأفضل تحديد حد لعدد الصفوف/الأعمدة (مثل وفقًا لـ [`MaxDataRow`](../../cells/maxdatarow/) و [`MaxDataColumn`](../../cells/maxdatacolumn/))، وإلا قد تزيد المصفوفة الكبيرة المرجعة من استهلاك الذاكرة بسبب كمية كبيرة من البيانات غير المفيدة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للسياق
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Formula = "=SUM(A1:C3)";

            try
            {
                // إنشاء خيارات الحساب باستخدام محرك مخصص
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ArrayModeCalculationEngine();
                workbook.CalculateFormula(options);

                Console.WriteLine("GetParamValueInArrayMode method called successfully");
                workbook.Save("GetParamValueInArrayModeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetParamValueInArrayMode: {ex.Message}");
            }
        }

        private class ArrayModeCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "SUM")
                {
                    // استدعِ GetParamValueInArrayMode مع معلمات واقعية
                    object[][] paramArray = data.GetParamValueInArrayMode(0, 5, 3);

                    Console.WriteLine($"Parameter array dimensions: {paramArray.Length} rows");
                    if (paramArray.Length > 0)
                    {
                        Console.WriteLine($"First row has {paramArray[0].Length} columns");
                    }
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


