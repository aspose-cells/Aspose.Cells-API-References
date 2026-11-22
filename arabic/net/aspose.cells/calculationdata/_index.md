---
title: "الفئة CalculationData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CalculationData. تمثل البيانات المطلوبة عند حساب دالة واحدة مثل اسم الدالة والمعلمات ...إلخ"
type: docs
url: /ar/net/aspose.cells/calculationdata/
---
## CalculationData class

يمثل البيانات المطلوبة عند حساب دالة واحدة، مثل اسم الدالة، المعلمات، ...إلخ.

```csharp
public class CalculationData
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue/) { get; set; } | يحصل أو يضبط القيمة المحسوبة لهذه الدالة. |
| [Cell](../../aspose.cells/calculationdata/cell/) { get; } | يحصل على كائن Cell حيث توجد الدالة. |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn/) { get; } | يحصل على فهرس العمود للخلية التي توجد فيها الدالة. |
| [CellRow](../../aspose.cells/calculationdata/cellrow/) { get; } | يحصل على فهرس الصف للخلية التي توجد فيها الدالة. |
| [FunctionName](../../aspose.cells/calculationdata/functionname/) { get; } | يحصل على اسم الدالة التي سيتم حسابها. |
| [ParamCount](../../aspose.cells/calculationdata/paramcount/) { get; } | يحصل على عدد المعلمات |
| [Workbook](../../aspose.cells/calculationdata/workbook/) { get; } | يحصل على كائن Workbook حيث توجد الدالة. |
| [Worksheet](../../aspose.cells/calculationdata/worksheet/) { get; } | يحصل على كائن Worksheet حيث توجد الدالة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext/)(int) | يحصل على النص الحرفي للمعامل عند الفهرس المحدد. |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue/)(int) | يحصل على كائن القيمة الممثلة للمعامل عند فهرس معين. |
| [GetParamValueInArrayMode](../../aspose.cells/calculationdata/getparamvalueinarraymode/)(int, int, int) | يحصل على القيمة (القيم) للمعامل عند فهرس معين. إذا كان المعامل نوعًا من التعبير يحتاج إلى حساب، فسيتم حسابه في وضع المصفوفة. |

### ملاحظات

جميع الكائنات التي توفرها هذه الفئة مخصصة لغرض \"القراءة\" فقط. يجب على المستخدم عدم تغيير أي بيانات في Workbook أثناء عملية حساب الصيغة، وإلا قد يحدث نتيجة غير متوقعة أو استثناء.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCalculationDataDemo
    {
        public static void Run()
        {
            try
            {
                // قم بإعداد دفتر عمل وورقة عمل بسيطين
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Name = "DemoSheet";

                // ضع بعض القيم التي ستُستخدم كمعلمات في دالة مخصصة
                sheet.Cells["A1"].PutValue(5);
                sheet.Cells["A2"].PutValue(10);

                // حدد صيغة تستدعي الدالة المخصصة
                sheet.Cells["B1"].Formula = "=MYFUNC(A1, A2)";

                // تكوين خيارات الحساب لاستخدام محرك مخصص
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new DemoEngine();

                // إجراء الحساب – سيستقبل المحرك المخصص كائنًا من نوع CalculationData
                workbook.CalculateFormula(options);

                // إخراج نتيجة الدالة المخصصة
                Console.WriteLine("Custom function result (B1): " + sheet.Cells["B1"].Value);

                // حفظ المصنف لإكمال العملية
                workbook.Save("CalculationDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with CalculationData: {ex.Message}");
            }
        }

        // محرك حساب مخصص يوضح الوصول إلى أعضاء CalculationData
        private class DemoEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // تأكد من أننا نتعامل مع الدالة المخصصة المتوقعة
                if (data.FunctionName != null &&
                    data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
                {
                    // استرجاع قيم المعاملات (يتم إرجاعها ككائنات)
                    object param0 = data.GetParamValue(0);
                    object param1 = data.GetParamValue(1);

                    // تحويل المعاملات إلى نوع double لإجراء الحساب
                    double val0 = Convert.ToDouble(param0);
                    double val1 = Convert.ToDouble(param1);
                    double result = val0 + val1; // simple addition

                    // تعيين النتيجة المحسوبة
                    data.CalculatedValue = result;

                    // إظهار قراءة الخصائص للقراءة فقط
                    Console.WriteLine("[Engine] FunctionName : " + data.FunctionName);
                    Console.WriteLine("[Engine] ParamCount   : " + data.ParamCount);
                    Console.WriteLine("[Engine] CellRow      : " + data.CellRow);
                    Console.WriteLine("[Engine] CellColumn   : " + data.CellColumn);
                }
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


