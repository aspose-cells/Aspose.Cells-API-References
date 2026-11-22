---
title: "Worksheet.CalculateArrayFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تحسب صيغة كصيغة مصفوفة"
type: docs
url: /ar/net/aspose.cells/worksheet/calculatearrayformula/
---
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}

يحسب صيغة كصيغة مصفوفة.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة التي سيتم حسابها. |
| opts | CalculationOptions | خيارات حساب الصيغة |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // املأ بعض بيانات العينة
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // تعريف صيغة مصفوفة
            string arrayFormula = "=SUM(A1:B3)";
            
            // احسب صيغة المصفوفة باستخدام خيارات الحساب
            object[][] result = worksheet.CalculateArrayFormula(arrayFormula, new CalculationOptions());
            
            // أخرج النتيجة.
            Console.WriteLine("Result of array formula calculation: " + result[0][0]);
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

## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}

يحسب صيغة كصيغة مصفوفة.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount, 
    int maxColumnCount)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة التي سيتم حسابها. |
| opts | CalculationOptions | خيارات حساب الصيغة |
| maxRowCount | Int32 | العدد الأقصى للصفوف للبيانات الناتجة. إذا كان غير موجب أو أكبر من عدد الصفوف الفعلي، فسيتم استخدام عدد الصفوف الفعلي. |
| maxColumnCount | Int32 | العدد الأقصى للأعمدة للبيانات الناتجة. إذا كان غير موجب أو أكبر من عدد الأعمدة الفعلي، فسيتم استخدام عدد الأعمدة الفعلي. |

### قيمة الإرجاع

نتيجة الصيغة المحسوبة.

### ملاحظات

سيتم اعتبار الصيغة كصيغة مصفوفة ديناميكية لحساب البُعد والنتيجة. يُستخدم البُعد الأقصى المحدد من قبل المستخدم في الحالات التي تكون فيها النتيجة المحسوبة مجموعة بيانات كبيرة (على سبيل المثال، قد تتطابق النتيجة المحسوبة مع بيانات صف كامل أو عمود كامل) لكن المستخدم لا يحتاج إلى مصفوفة كبيرة وفقًا لمتطلبات العمل أو لأسباب تتعلق بالأداء.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsInt32IDemo
    {
        public static void Run()
        {
            // إنشاء مصنف والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // مثال 1: حساب صيغة مصفوفة بسيطة
            string formula = "=ISBLANK(IF(TRUE,B2:B5))";
            CalculationOptions options = new CalculationOptions();
            object[][] result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of ISBLANK(IF(TRUE,B2:B5)): " + result[0][0]);

            // مثال 2: صيغة مصفوفة بنطاق ديناميكي
            formula = "=LEN(IF({1;2;3;4},B2:B5))";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of LEN(IF({1;2;3;4},B2:B5)): " + result[0][0]);

            // مثال 3: صيغة مصفوفة مع دالة MATCH
            // إعداد بعض بيانات الاختبار
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(10);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["C3"].PutValue(2);
            sheet.Cells["D2"].PutValue(0);
            sheet.Cells["D3"].PutValue(0);

            formula = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of MATCH formula: " + result[0][0]);
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

## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}

يحسب صيغة كصيغة مصفوفة.

```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts, 
    CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, 
    int maxColumnCount, CalculationData calculationData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة التي سيتم حسابها. |
| pOpts | FormulaParseOptions | خيارات تحليل الصيغة |
| cOpts | CalculationOptions | خيارات حساب الصيغة |
| baseCellRow | Int32 | فهرس الصف للخلية الأساسية. |
| baseCellColumn | Int32 | فهرس العمود للخلية الأساسية. |
| maxRowCount | Int32 | الحد الأقصى لعدد الصفوف للبيانات الناتجة. إذا كان غير إيجابي أو أكبر من عدد الصفوف الفعلي، فسيتم استخدام عدد الصفوف الفعلي. |
| maxColumnCount | Int32 | الحد الأقصى لعدد الأعمدة للبيانات الناتجة. إذا كان غير إيجابي أو أكبر من عدد الصفوف الفعلي، فسيتم استخدام عدد الأعمدة الفعلي. |
| calculationData | CalculationData | بيانات الحساب. تُستخدم في الحالة التي يحتاج فيها المستخدم إلى حساب بعض الصيغ الثابتة عند تنفيذ محرك حساب مخصص. لهذا النوع من الحالات، يحتاج المستخدم إلى تحديدها باستخدام بيانات الحساب المقدمة لـ [`Calculate`](../../abstractcalculationengine/calculate/). |

### قيمة الإرجاع

نتيجة الصيغة المحسوبة.

### ملاحظات

سيتم اعتبار الصيغة كصيغة مصفوفة ديناميكية لحساب البُعد والنتيجة. يُستخدم البُعد الأقصى المحدد من قبل المستخدم في الحالات التي تكون فيها النتيجة المحسوبة مجموعة بيانات كبيرة (على سبيل المثال، قد تتطابق النتيجة المحسوبة مع بيانات صف كامل أو عمود كامل) لكن المستخدم لا يحتاج إلى مصفوفة كبيرة وفقًا لمتطلبات العمل أو لأسباب تتعلق بالأداء.

### انظر أيضًا

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


