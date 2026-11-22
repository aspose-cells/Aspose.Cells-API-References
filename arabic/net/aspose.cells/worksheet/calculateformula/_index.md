---
title: "Worksheet.CalculateFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تحسب صيغة"
type: docs
url: /ar/net/aspose.cells/worksheet/calculateformula/
---
## CalculateFormula(string) {#calculateformula}

يحسب صيغة.

```csharp
public object CalculateFormula(string formula)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة التي سيتم حسابها. |

### قيمة الإرجاع

نتيجة الصيغة المحسوبة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Worksheet sheet = wb.Worksheets[0];

            // توضيح تحويل الأعداد الأساسي
            string formula = "=NUMBERVALUE(\"1.234\")";
            Console.WriteLine("NUMBERVALUE(\"1.234\") = " + sheet.CalculateFormula(formula));

            // توضيح تحويل العملات
            formula = "=NUMBERVALUE(\"$1,234.56\")";
            Console.WriteLine("NUMBERVALUE(\"$1,234.56\") = " + sheet.CalculateFormula(formula));

            // توضيح تحويل الوقت
            formula = "=NUMBERVALUE(\"0:25\")";
            Console.WriteLine("NUMBERVALUE(\"0:25\") = " + sheet.CalculateFormula(formula));

            // توضيح تحويل التاريخ
            formula = "=NUMBERVALUE(\"07/26/2023\")";
            Console.WriteLine("NUMBERVALUE(\"07/26/2023\") = " + sheet.CalculateFormula(formula));

            // توضيح حالة الخطأ
            formula = "=NUMBERVALUE(\"invalid\")";
            Console.WriteLine("NUMBERVALUE(\"invalid\") = " + sheet.CalculateFormula(formula));
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, CalculationOptions) {#calculateformula_1}

يحسب تعبير الصيغة مباشرة.

```csharp
public object CalculateFormula(string formula, CalculationOptions opts)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة التي سيتم حسابها. |
| opts | CalculationOptions | خيارات حساب الصيغة |

### قيمة الإرجاع

نتيجة الصيغة المعطاة المحسوبة. قد يكون الكائن المرتجع من أحد الأنواع الممكنة لـ [`Value`](../../cell/value/)، أو ReferredArea.

### ملاحظات

سيتم حساب الصيغة كما تم تعيينها في الخلية A1. وستُعامل الصيغة كصيغة عادية. إذا كنت بحاجة إلى حساب الصفة كصيغة مصفوفة والحصول على مصفوفة للنتيجة المحسوبة، يرجى استخدام [`CalculateArrayFormula`](../calculatearrayformula/) بدلاً من ذلك.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // املأ بعض بيانات العينة
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // إنشاء محرك حساب مخصص
            CustomEngine customEngine = new CustomEngine();
            
            // احسب الصيغة باستخدام محرك مخصص
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };
            
            object result = worksheet.CalculateFormula("=SUM(A1:A3)", options);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object value = data.GetParamValue(i);
                    if (value is double)
                    {
                        sum += (double)value;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### انظر أيضًا

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) {#calculateformula_2}

يحسب تعبير الصيغة مباشرة.

```csharp
public object CalculateFormula(string formula, FormulaParseOptions pOpts, CalculationOptions cOpts, 
    int baseCellRow, int baseCellColumn, CalculationData calculationData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة التي سيتم حسابها. |
| pOpts | FormulaParseOptions | خيارات تحليل الصيغة. |
| cOpts | CalculationOptions | خيارات حساب الصيغة. |
| baseCellRow | Int32 | فهرس الصف للخلية الأساسية. |
| baseCellColumn | Int32 | فهرس العمود للخلية الأساسية. |
| calculationData | CalculationData | بيانات الحساب. تُستخدم في الحالة التي يحتاج فيها المستخدم إلى حساب بعض الصيغ الثابتة عند تنفيذ محرك حساب مخصص. لهذا النوع من الحالات، يحتاج المستخدم إلى تحديدها باستخدام بيانات الحساب المقدمة لـ [`Calculate`](../../abstractcalculationengine/calculate/). |

### قيمة الإرجاع

نتيجة الصيغة المعطاة المحسوبة. قد يكون الكائن المرتجع من أحد الأنواع الممكنة لـ [`Value`](../../cell/value/)، أو ReferredArea.

### ملاحظات

سيتم حساب الصيغة كما تم تعيينها إلى الخلية الأساسية المحددة. وستُعامل الصيغة كصيغة عادية. إذا كنت بحاجة إلى حساب الصيغة كصيغة مصفوفة والحصول على مصفوفة للنتيجة المحسوبة، يرجى استخدام [`CalculateArrayFormula`](../calculatearrayformula/) بدلاً من ذلك.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringFormulaParseOptCalculati169472Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بيانات عينة
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C1"].PutValue(2);
            worksheet.Cells["C2"].PutValue(4);

            // تعريف خيارات الحساب
            CalculationOptions calculationOptions = new CalculationOptions();
            
            // تعريف خيارات تحليل الصيغة
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions();
            
            // احسب الصيغة بجميع المعلمات
            object result = worksheet.CalculateFormula(
                "=SUM(B1:B2, C1:C2)",  // formula
                formulaParseOptions,   // parse options
                calculationOptions,    // calculation options
                0,                     // base cell row
                0,                     // base cell column
                null                   // calculation data
            );

            // أخرج النتيجة.
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### انظر أيضًا

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions, bool) {#calculateformula_3}

يحسب جميع الصيغ في هذه ورقة العمل.

```csharp
public void CalculateFormula(CalculationOptions options, bool recursive)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | CalculationOptions | خيارات الحساب |
| recursive | منطقي | True يعني إذا كانت خلايا ورقة العمل تعتمد على خلايا أوراق عمل أخرى، فسيتم حساب الخلايا التابعة في الأوراق الأخرى أيضًا. False يعني أنه تم حساب جميع الصيغ في ورقة العمل والقيم صحيحة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithCalculationOptionsBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين بيانات وعينات الصيغ
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue("=SUM(A1:A3)");
            
            // إنشاء خيارات الحساب
            CalculationOptions options = new CalculationOptions();
            options.Recursive = true;
            options.IgnoreError = false;
            
            // احسب الصيغة باستخدام الخيارات وإجبار حساب كامل
            worksheet.CalculateFormula(options, true);
            
            // إخراج النتيجة المحسوبة
            Console.WriteLine("Calculated value: " + worksheet.Cells["B1"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


