---
title: "Cell.SetArrayFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تعيين صيغة مصفوفة إلى نطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells/cell/setarrayformula/
---
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}

يضبط صيغة مصفوفة لنطاق من الخلايا.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | String | صيغة مصفوفة. |
| rowNumber | Int32 | عدد الصفوف لملء نتيجة صيغة المصفوفة. |
| columnNumber | Int32 | عدد الأعمدة لملء نتيجة صيغة المصفوفة. |
| isR1C1 | منطقي | ما إذا كانت الصيغة بصيغة R1C1 |
| isLocal | منطقي | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. |

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.SetArrayFormula(string,int,int,FormulaParseOptions). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2019. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetArrayFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;

            try
            {
                // احصل على الخلية المستهدفة حيث نريد تعيين صيغة المصفوفة
                Cell targetCell = worksheet.Cells["B1"];

                // عيّن صيغة مصفوفة تضرب القيم في A1:A3 في 2
                // المعلمات: (formula, rowNumber=3, columnNumber=1, isR1C1=false, isLocal=false)
                targetCell.SetArrayFormula("=A1:A3*2", 3, 1, false, false);

                // احسب المصنف لرؤية النتائج
                workbook.CalculateFormula();

                // عرض النتائج
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B2 value: {worksheet.Cells["B2"].Value}");
                Console.WriteLine($"B3 value: {worksheet.Cells["B3"].Value}");

                // احفظ المصنف
                workbook.Save("SetArrayFormulaDemo.xlsx");
                Console.WriteLine("Array formula set successfully and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting array formula: {ex.Message}");
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

## SetArrayFormula(string, int, int) {#setarrayformula}

يضبط صيغة مصفوفة (صيغة مصفوفة قديمة تُدخل عبر CTRL+SHIFT+ENTER في مايكروسوفت إكسل) لنطاق من الخلايا.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | String | صيغة مصفوفة. |
| rowNumber | Int32 | عدد الصفوف لملء نتيجة صيغة المصفوفة. |
| columnNumber | Int32 | عدد الأعمدة لملء نتيجة صيغة المصفوفة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            Cell cell = cells["A1"];
            cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);

            workbook.CalculateFormula();

            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1} value: {cells[i, 0].IntValue}");
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

## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}

يضبط صيغة مصفوفة لنطاق من الخلايا.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | String | صيغة مصفوفة. |
| rowNumber | Int32 | عدد الصفوف لملء نتيجة صيغة المصفوفة. |
| columnNumber | Int32 | عدد الأعمدة لملء نتيجة صيغة المصفوفة. |
| خيارات | FormulaParseOptions | خيارات تحليل الصيغة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ضع بيانات عينة في الخلايا C1:E1
            cells["C1"].PutValue(10);
            cells["D1"].PutValue(20);
            cells["E1"].PutValue(30);

            // عيّن صيغة مصفوفة في الخلية A1 التي ستمتد إلى صفين و3 أعمدة
            cells["A1"].SetArrayFormula("=TRANSPOSE(C1:E1)", 2, 1, new FormulaParseOptions());

            // حساب الصيغ
            workbook.CalculateFormula();

            // أخرج النتائج
            Console.WriteLine("Array formula results:");
            for (int row = 0; row < 2; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = cells[row, col];
                    Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                }
            }
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

## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}

يضبط صيغة مصفوفة لنطاق من الخلايا.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| arrayFormula | String | صيغة مصفوفة. |
| rowNumber | Int32 | عدد الصفوف لملء نتيجة صيغة المصفوفة. |
| columnNumber | Int32 | عدد الأعمدة لملء نتيجة صيغة المصفوفة. |
| خيارات | FormulaParseOptions | خيارات تحليل الصيغة. |
| القيم | Object[][] | القيم لتلك الخلايا مع صيغة المصفوفة المعطاة |

### انظر أيضًا

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


