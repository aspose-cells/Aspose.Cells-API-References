---
title: "AbstractCalculationEngine.IsParamLiteralRequired"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractCalculationEngine. تشير إلى ما إذا كان هذا المحرك يحتاج إلى النص الحرفي للمعامل أثناء إجراء حساب. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/abstractcalculationengine/isparamliteralrequired/
---
## AbstractCalculationEngine.IsParamLiteralRequired property

يشير إلى ما إذا كان هذا المحرك يحتاج إلى النص الحرفي للمعامل أثناء إجراء الحساب. القيمة الافتراضية هي false.

```csharp
public virtual bool IsParamLiteralRequired { get; }
```

### ملاحظات

إذا كان هذا المحرك الحسابي المخصص يحتاج إلى النص الحرفي للمعامل، فستحتاج المزيد من المكدسات لتخزين النص الحرفي للمعاملات وقد يتم استدعاء طريقة Calculate() بشكل متكرر لحساب قيمة المعامل. عمومًا، لا يُحتاج إلى النص الحرفي لحساب الصيغ ويجب إبقاء هذه الخاصية على false في معظم التطبيقات للحصول على أداء أفضل.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyIsParamLiteralRequiredDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مثال لمحرك حساب مخصص
            MyCustomEngine engine = new MyCustomEngine();

            // قراءة قيمة الخاصية الحالية
            Console.WriteLine("Current IsParamLiteralRequired value: " + engine.IsParamLiteralRequired);

            // إنشاء صيغة اختبار مع معامل نصي حرفي
            worksheet.Cells["A1"].Formula = "=MYFUNC(\"123\")";

            // احسب المصنف باستخدام خيارات حساب مخصصة
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            // اعرض نتيجة الحساب بناءً على قيمة الخاصية
            Console.WriteLine("Formula result: " + worksheet.Cells["A1"].StringValue);

            workbook.Save("IsParamLiteralRequiredDemo.xlsx");
        }
    }

    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override bool IsParamLiteralRequired => true;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
            {
                if (data.ParamCount > 0)
                {                    
                    object paramValue = data.GetParamValue(0);
                    string result = (paramValue is string) ? "Literal received" : "Value received";
                    data.CalculatedValue = result;
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


