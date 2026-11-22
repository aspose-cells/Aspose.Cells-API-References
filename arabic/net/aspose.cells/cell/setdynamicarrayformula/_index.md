---
title: "Cell.SetDynamicArrayFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تعين صيغة مصفوفة ديناميكية وتجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا"
type: docs
url: /ar/net/aspose.cells/cell/setdynamicarrayformula/
---
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}

يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    bool calculateValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | String | تعبير الصيغة |
| خيارات | FormulaParseOptions | خيارات لتحليل الصيغة. سيتم تجاهل خيار "Parse" وستتم دائمًا تحليل الصيغة فورًا |
| calculateValue | منطقي | ما إذا كان سيتم حساب هذه الصيغة الديناميكية للمصفوفة لتلك الخلايا في النطاق المتسرب. |

### قيمة الإرجاع

النطاق الذي يجب أن تتسرب إليه الصيغة.

### ملاحظات

قد لا يكون النطاق المعاد هو نفسه النطاق الفعلي الذي تتسرب إليه هذه الصيغة الديناميكية للمصفوفة. إذا كان هناك خلايا غير فارغة في النطاق، سيتم تعيين الصيغة للخلية الحالية فقط وت标ها كـ "#SPILL!". ولكن في مثل هذه الحالة ما زلنا نعيد النطاق الكامل الذي يجب أن تتسرب إليه هذه الصيغة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsBooleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // تعيين صيغة مصفوفة ديناميكية في الخلية A1
            Cell cell1 = cells["A1"];
            cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);

            // تعيين قيمة في B2 ستؤثر على صيغة SEQUENCE
            cells["B2"].PutValue(3);

            // حساب الصيغ وتحديث المصفوفات الديناميكية
            wb.CalculateFormula();
            wb.RefreshDynamicArrayFormulas(false);

            // إخراج النتائج من النطاق المتسرب
            Console.WriteLine("Dynamic array results:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine(cells[0, i].Value);
            }
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}

يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | String | تعبير الصيغة |
| خيارات | FormulaParseOptions | خيارات لتحليل الصيغة. سيتم تجاهل خيار "Parse" وستتم دائمًا تحليل الصيغة فورًا |
| القيم | Object[][] | القيم (النتائج المحسوبة) لتلك الخلايا التي لديها صيغة مصفوفة ديناميكية معينة |
| calculateRange | منطقي | ما إذا كان سيتم حساب النطاق المتسرب لهذه الصيغة الديناميكية للمصفوفة. إذا كان معامل "values" غير فارغ وكان هذا العلم false، فإن ارتفاع النطاق المتسرب سيكون values.Length وعرضه سيكون values[0].Length. |
| calculateValue | منطقي | ما إذا كان سيتم حساب هذه الصيغة الديناميكية للمصفوفة لتلك الخلايا في النطاق المتسرب عندما يكون "values" فارغًا أو العنصر المقابل في "values" لخلية واحدة فارغًا. |

### قيمة الإرجاع

النطاق الذي يجب أن تتسرب إليه الصيغة.

### ملاحظات

قد لا يكون النطاق المعاد هو نفسه النطاق الفعلي الذي تتسرب إليه هذه الصيغة الديناميكية للمصفوفة. إذا كان هناك خلايا غير فارغة في النطاق، سيتم تعيين الصيغة للخلية الحالية فقط وت标ها كـ "#SPILL!". ولكن في مثل هذه الحالة ما زلنا نعيد النطاق الكامل الذي يجب أن تتسرب إليه هذه الصيغة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue(10);
            cell = cells["A2"];
            cell.PutValue(20);
            cell = cells["B1"];
            cell.PutValue(60);
            cell = cells["B2"];
            cell.PutValue(80);

            // احصل على الخلية C1 حيث سيتم تعيين الصيغة الديناميكية للمصفوفة
            cell = worksheet.Cells["C1"];

            // تعريف الصيغة الديناميكية للمصفوفة
            string formula = "=A1:B2 * 2";
            
            // إنشاء خيارات تحليل الصيغة
            FormulaParseOptions options = new FormulaParseOptions
            {
                Parse = true // Enable formula parsing
            };

            // تحضير القيم لملء خلايا نتائج الصيغة
            object[][] values = new object[2][];
            values[0] = new object[] { 2, 4 };
            values[1] = new object[] { 6, 8 };

            try
            {
                // تعيين صيغة مصفوفة ديناميكية بقيم مسبقة الحساب
                CellArea result = cell.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange: false,  // Use values array dimensions for spill range
                    calculateValue: false  // Use provided values instead of calculating
                );

                Console.WriteLine($"Dynamic array formula set. Affected range: Rows {result.StartRow}-{result.EndRow}, Columns {result.StartColumn}-{result.EndColumn}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula: {ex.Message}");
            }

            // حفظ المصنف مع التغييرات
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) {#setdynamicarrayformula_2}

يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | String | تعبير الصيغة |
| خيارات | FormulaParseOptions | خيارات لتحليل الصيغة. سيتم تجاهل خيار "Parse" وستتم دائمًا تحليل الصيغة فورًا |
| القيم | Object[][] | القيم (النتائج المحسوبة) لتلك الخلايا التي لديها صيغة مصفوفة ديناميكية معينة |
| calculateRange | منطقي | ما إذا كان سيتم حساب النطاق المتسرب لهذه الصيغة الديناميكية للمصفوفة. إذا كان معامل "values" غير فارغ وكان هذا العلم false، فإن ارتفاع النطاق المتسرب سيكون values.Length وعرضه سيكون values[0].Length. |
| calculateValue | منطقي | ما إذا كان سيتم حساب هذه الصيغة الديناميكية للمصفوفة لتلك الخلايا في النطاق المتسرب عندما يكون "values" فارغًا أو العنصر المقابل في "values" لخلية واحدة فارغًا. |
| copts | CalculationOptions | خيارات حساب الصيغة. عادةً، لأسباب تتعلق بالأداء، يجب أن تكون الخاصية [`Recursive`](../../calculationoptions/recursive/) مساوية لـ false. |

### قيمة الإرجاع

النطاق الذي يجب أن تتسرب إليه الصيغة.

### ملاحظات

قد لا يكون النطاق المعاد هو نفسه النطاق الفعلي الذي تتسرب إليه هذه الصيغة الديناميكية للمصفوفة. إذا كان هناك خلايا غير فارغة في النطاق، سيتم تعيين الصيغة للخلية الحالية فقط وت标ها كـ "#SPILL!". ولكن في مثل هذه الحالة ما زلنا نعيد النطاق الكامل الذي يجب أن تتسرب إليه هذه الصيغة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة في الخلايا A2:B5
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B3"].PutValue(55);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["B5"].PutValue(70);

            // احصل على الخلية الهدف D1
            Cell cellD1 = worksheet.Cells["D1"];

            try
            {
                // تحضير المعلمات لـ SetDynamicArrayFormula
                string formula = "=FILTER(A2:A5, B2:B5>50)";
                FormulaParseOptions options = new FormulaParseOptions { Parse = true };
                object[][] values = new object[2][] { new object[] { 10 }, new object[] { 40 } };
                bool calculateRange = true;
                bool calculateValue = true;
                CalculationOptions calcOptions = new CalculationOptions { Recursive = true };

                // استدعِ SetDynamicArrayFormula مع معلمات محددة
                CellArea spillRange = cellD1.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange,
                    calculateValue,
                    calcOptions
                );

                Console.WriteLine($"Dynamic array formula set successfully. Spill range: {spillRange}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


