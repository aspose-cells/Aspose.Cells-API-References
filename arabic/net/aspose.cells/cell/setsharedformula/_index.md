---
title: "Cell.SetSharedFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة الخلية. تعيين صيغة لنطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells/cell/setsharedformula/
---
## SetSharedFormula(string, int, int, bool, bool) {#setsharedformula_3}

يعيّن صيغة لنطاق من الخلايا.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sharedFormula | String | صيغة مشتركة. |
| rowNumber | Int32 | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | Int32 | عدد الأعمدة لتعبئة الصيغة. |
| isR1C1 | منطقي | ما إذا كانت الصيغة بصيغة R1C1 |
| isLocal | منطقي | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. |

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.SetSharedFormula(string,int,int,FormulaParseOptions). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2019. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            // تعبئة بيانات عينة في العمود A
            for (int row = 0; row < 5; row++)
            {
                cells[row, 0].Value = row + 1; // A1-A5: 1-5
            }

            // احصل على الخلية المستهدفة B1 لتعيين الصيغة المشتركة
            Cell targetCell = cells[0, 1]; // B1

            try
            {
                // تعيين الصيغة المشتركة لحساب مربع القيم في العمود A
                // المعلمات: (formula, rowCount=5, columnCount=1, isR1C1=false, isLocal=false)
#pragma warning disable 0618 // Disable obsolete warning for demonstration
                targetCell.SetSharedFormula("=A1^2", 5, 1, false, false);
#pragma warning restore 0618

                // تحقق من انتشار الصيغة
                Console.WriteLine($"B1 formula: {targetCell.Formula}");
                Console.WriteLine($"B5 formula: {cells[4, 1].Formula}");

                // احسب المصنف لتحديث نتائج الصيغة
                workbook.CalculateFormula();

                Console.WriteLine($"A1 value: {cells["A1"].Value}");
                Console.WriteLine($"A5 value: {cells["A5"].Value}");
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B5 value: {cells[4, 1].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
                return;
            }

            // احفظ المصنف المعدل
            workbook.Save("SetSharedFormulaDemo.xlsx");
            Console.WriteLine("Spreadsheet saved successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int) {#setsharedformula}

يضبط صيغًا مشتركة لنطاق من الخلايا.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sharedFormula | String | صيغة مشتركة. |
| rowNumber | Int32 | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | Int32 | عدد الأعمدة لتعبئة الصيغة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetSharedFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين صيغة مشتركة في العمود B بدءًا من B1 إلى B20
            cells["B1"].SetSharedFormula("=C1*2", 20, 1);

            // تعيين بعض القيم في العمود C لتوضيح حساب الصيغة
            for (int i = 0; i < 20; i++)
            {
                cells[i, 2].PutValue(i + 1); // Column C values (C1=1, C2=2...)
            }

            // حساب الصيغ
            workbook.CalculateFormula();

            // إخراج النتائج للتحقق
            for (int i = 0; i < 5; i++) // Display first 5 results
            {
                Console.WriteLine($"B{i+1} value: {cells[i, 1].Value}");
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

## SetSharedFormula(string, int, int, FormulaParseOptions) {#setsharedformula_1}

يضبط صيغًا مشتركة لنطاق من الخلايا.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sharedFormula | String | صيغة مشتركة. |
| rowNumber | Int32 | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | Int32 | عدد الأعمدة لتعبئة الصيغة. |
| خيارات | FormulaParseOptions | خيارات تحليل الصيغة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعبئة بيانات عينة في العمود A
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // احصل على الخلية المستهدفة حيث سنقوم بتعيين الصيغة المشتركة
            Cell targetCell = worksheet.Cells["B1"];

            try
            {
                // إنشاء خيارات تحليل الصيغة بالإعدادات الافتراضية
                FormulaParseOptions options = new FormulaParseOptions();

                // تعيين صيغة مشتركة لثلاث صفوف وعمودين بدءًا من B1
                targetCell.SetSharedFormula("=A1*2", 3, 2, options);

                Console.WriteLine("Shared formula set successfully for B1:C3 range");
                Console.WriteLine("B1 formula: " + worksheet.Cells["B1"].Formula);
                Console.WriteLine("C3 formula: " + worksheet.Cells["C3"].Formula);

                workbook.CalculateFormula();
                Console.WriteLine("B3 value: " + worksheet.Cells["B3"].Value);
                Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
                Console.WriteLine("C3 value: " + worksheet.Cells["C3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("SetSharedFormulaDemo.xlsx");
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

## SetSharedFormula(string, int, int, FormulaParseOptions, object[][]) {#setsharedformula_2}

يضبط صيغًا مشتركة لنطاق من الخلايا.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sharedFormula | String | صيغة مشتركة. |
| rowNumber | Int32 | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | Int32 | عدد الأعمدة لتعبئة الصيغة. |
| خيارات | FormulaParseOptions | خيارات تحليل الصيغة. |
| القيم | Object[][] | القيم لتلك الخلايا مع الصيغة المشتركة المحددة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo1
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين قيمة عينة في الخلية A1
            worksheet.Cells["A1"].PutValue(5);

            // الحصول على الخلية الهدف B2 حيث سيتم تعيين الصيغة المشتركة
            Cell cell = worksheet.Cells["B2"];

            try
            {
                // تحديد معلمات الصيغة المشتركة
                string formula = "=A1*2";
                int totalRows = 2;
                int totalColumns = 2;
                FormulaParseOptions parseOptions = new FormulaParseOptions();
                object[][] presetValues = new object[2][]
                {
                    new object[] { 10, 10 },
                    new object[] { 10, 10 }
                };

                // تعيين الصيغة المشتركة لنطاق 2×2 يبدأ من B2 مع القيم المحددة مسبقًا
                cell.SetSharedFormula(formula, totalRows, totalColumns, parseOptions, presetValues);

                Console.WriteLine("Shared formula set successfully. Cells B2:C3 contain values 10");
                workbook.CalculateFormula();
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "C3");
                IEnumerator iter = range.GetEnumerator();
                while(iter.MoveNext()) 
                {
                    Cell temp = (Cell)iter.Current;
                    Console.WriteLine(temp.Name + "  " + temp.Value);
                }

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("SetSharedFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


