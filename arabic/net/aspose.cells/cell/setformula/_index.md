---
title: "Cell.SetFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تعيين الصيغة والنتيجة المحسوبة للصيغة"
type: docs
url: /ar/net/aspose.cells/cell/setformula/
---
## SetFormula(string, object) {#setformula_3}

يضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة.

```csharp
public void SetFormula(string formula, object value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة. |
| القيمة | Object | القيمة (النتيجة المحسوبة) للصيغة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringObjectDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين الصيغة باستخدام معلمات string و object
            cells["A1"].SetFormula("=SUM(1,2)", 4); // Will display 4 until calculation
            cells["A2"].SetFormula("=AVERAGE(5,10)", 7.5); // Will display 7.5 until calculation

            // عرض القيم قبل الحساب
            Console.WriteLine("Before Calculation:");
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);

            // حساب الصيغ
            workbook.CalculateFormula();

            // عرض القيم بعد الحساب
            Console.WriteLine("\nAfter Calculation:");
            Console.WriteLine("A1: " + cells["A1"].IntValue); // Should show 3
            Console.WriteLine("A2: " + cells["A2"].DoubleValue); // Should show 7.5
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions) {#setformula}

يضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة.

```csharp
public void SetFormula(string formula, FormulaParseOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة. |
| خيارات | FormulaParseOptions | خيارات تحليل الصيغة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على خلية محددة (B2 في هذه الحالة)
            Cell cell = worksheet.Cells["B2"];
            
            // تعيين بعض القيم الأولية للتوضيح
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            
            // مثال 1: تعيين صيغة بسيطة مع خيارات التحليل الافتراضية
            cell.SetFormula("=SUM(A1:A2)", new FormulaParseOptions());
            Console.WriteLine("Formula with default options: " + cell.Formula);
            
            // مثال 2: تعيين الصيغة بنمط R1C1 باستخدام FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            
            cell.SetFormula("=SUM(R[-1]C[-1]:R[0]C[-1])", options);
            Console.WriteLine("Formula with R1C1 style: " + cell.Formula);
            
            // مثال 3: تعيين الصيغة باستخدام خيارات التحليل التي تحافظ على تنسيق R1C1
            options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            cell.SetFormula("=R1C1+R2C2", options);
            Console.WriteLine("Formula preserved as R1C1: " + cell.Formula);
            
            // احسب المصنف لرؤية النتائج
            workbook.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.Value);
        }
    }
}
```

### انظر أيضًا

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, bool, bool, object) {#setformula_2}

عيّن الصيغة وقيمة الصيغة.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetFormula(string formula, bool isR1C1, bool isLocal, object value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة. |
| isR1C1 | منطقي | ما إذا كانت الصيغة صيغة R1C1. |
| isLocal | منطقي | ما إذا كانت الصيغة مُنسقة محليًا. |
| القيمة | Object | قيمة الصيغة. |

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.SetFormula(string,FormulaParseOptions,object). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2019. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetFormulaWithStringBooleanBooleanObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);

            // احصل على الخلية المستهدفة حيث سنقوم بتعيين الصيغة
            Cell cell = worksheet.Cells["C1"];

            try
            {
                // تعيين صيغة مع جميع المعلمات
                // المعلمات: سلسلة الصيغة، isR1C1، isLocal، القيمة
                cell.SetFormula("=SUM(A1:B2)", false, false, null);

                // احسب الصيغة
                workbook.CalculateFormula();

                // اعرض النتيجة
                Console.WriteLine($"Formula set successfully. Result: {cell.Value}");

                // احفظ المصنف
                workbook.Save("SetFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting formula: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions, object) {#setformula_1}

يضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة.

```csharp
public void SetFormula(string formula, FormulaParseOptions options, object value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة. |
| خيارات | FormulaParseOptions | خيارات تحليل الصيغة. |
| القيمة | Object | القيمة (النتيجة المحسوبة) للصيغة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // تعيين الصيغة الأولية مع إشارة الإضافة
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Initial formula: " + sheet.Cells[0, 0].Formula);

            // استخدم SetFormula لتجاوز دون التحقق من الإضافة
            sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
            Console.WriteLine("After SetFormula: " + sheet.Cells[0, 0].Formula);

            // إعادة الضبط إلى صيغة الإضافة
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Reset to add-in formula: " + sheet.Cells[0, 0].Formula);

            // إنشاء مصنف جديد ونسخ الورقة
            Workbook wb2 = new Workbook();
            wb2.Worksheets[0].Cells[0, 0].Formula = "'externalDS.xlam'!dsfunnew(C1)";
            wb2.Worksheets[0].Copy(sheet);
            Console.WriteLine("After copy: " + wb2.Worksheets[0].Cells[0, 0].Formula);
        }
    }
}
```

### انظر أيضًا

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


