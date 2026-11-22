---
title: "الفئة AbstractCalculationEngine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.AbstractCalculationEngine. تمثل محرك حساب مخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells"
type: docs
url: /ar/net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

يمثل محرك الحساب المخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

```csharp
public abstract class AbstractCalculationEngine
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [IsParamArrayModeRequired](../../aspose.cells/abstractcalculationengine/isparamarraymoderequired/) { get; } | يشير إلى ما إذا كان هذا المحرك يحتاج إلى حساب المعامل في وضع المصفوفة. القيمة الافتراضية هي false. إذا كان [`GetParamValueInArrayMode`](../calculationdata/getparamvalueinarraymode/) مطلوبًا عند حساب الدوال المخصصة ولم يقم المستخدم بتحديث التعريف لها (باستخدام [`UpdateCustomFunctionDefinition`](../workbook/updatecustomfunctiondefinition/))، يجب تعيين هذه الخاصية إلى true. |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired/) { get; } | يشير إلى ما إذا كان هذا المحرك يحتاج إلى النص الحرفي للمعامل أثناء إجراء الحساب. القيمة الافتراضية هي false. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions/) { get; } | ما إذا كان يجب فحص ومعالجة الدوال المدمجة التي يدعمها المحرك المدمج بواسطة هذا التنفيذ. القيمة الافتراضية هي false. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate/)(CalculationData) | يحسب دالة واحدة باستخدام البيانات المعطاة. |
| virtual [ForceRecalculate](../../aspose.cells/abstractcalculationengine/forcerecalculate/)(string) | ما إذا كان يجب إجبار الدالة المعطاة على إعادة حسابها دائمًا عند حساب الصيغ المشتركة. |
| [SkipCalculation](../../aspose.cells/abstractcalculationengine/skipcalculation/)() | يتخطى الحساب للمعادلة بالكامل التي تشير إلى الدالة التي يتم تقييمها حاليًا. |

### ملاحظات

يجب على المستخدم عدم تعديل أي جزء من المصنف مباشرةً في هذا التنفيذ (باستثناء النتيجة المحسوبة للدالة المخصصة، والتي يمكن تعيينها عبر خاصية CalculationData.CalculatedValue). وإلا قد يحدث نتيجة غير متوقعة أو استثناء. إذا كان المستخدم بحاجة إلى تغيير بيانات أخرى غير النتيجة المحسوبة في التنفيذ لبعض الدوال المخصصة، على سبيل المثال، تغيير صيغة الخلية أو النمط ... إلخ، يجب على المستخدم جمع تلك البيانات في هذا التنفيذ وتغييرها خارج نطاق حساب الصيغ.

### أمثلة

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // مثال: تنفيذ مخصص لدالة باسم "MYFUNC"
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                // افترض أن MYFUNC تأخذ معاملين وتعيد مجموعهما
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            // إجبار إعادة الحساب للدالة المخصصة "MYFUNC"
            return functionName.ToUpper() == "MYFUNC";
        }
    }

    public class CalculationEngineDemo
    {
        public static void Test()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // ضع بعض القيم في الخلايا
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);

            // أضف صيغة تستخدم الدالة المخصصة
            sheet.Cells["A3"].Formula = "=MYFUNC(A1, A2)";

            // حدد خيارات الحساب باستخدام المحرك المخصص
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = new CustomCalculationEngine(),
                IgnoreError = false,
                Recursive = true
            };

            // احسب الصيغ باستخدام المحرك المخصص
            workbook.CalculateFormula(options);

            // اطبع نتيجة الدالة المخصصة
            Console.WriteLine("Result of MYFUNC(A1, A2): " + sheet.Cells["A3"].Value);

            // احفظ المصنف
            workbook.Save("CustomCalculationEngineExample.xlsx");
            workbook.Save("CustomCalculationEngineExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


