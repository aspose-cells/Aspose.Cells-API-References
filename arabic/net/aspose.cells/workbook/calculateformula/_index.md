---
title: "Workbook.CalculateFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تحسب نتيجة الصيغ"
type: docs
url: /ar/net/aspose.cells/workbook/calculateformula/
---
## CalculateFormula() {#calculateformula}

يحسب نتيجة الصيغ.

```csharp
public void CalculateFormula()
```

### ملاحظات

لجميع الصيغ المدعومة، يرجى الاطلاع على القائمة في https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // تعيين القيم والصيغ
            cells["A1"].PutValue(5);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=B1+10";
            
            // حساب الصيغ
            workbook.CalculateFormula();
            
            // عرض النتائج
            Console.WriteLine("A1 value: " + cells["A1"].IntValue);
            Console.WriteLine("B1 formula result: " + cells["B1"].IntValue);
            Console.WriteLine("C1 formula result: " + cells["C1"].IntValue);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(bool) {#calculateformula_2}

يحسب نتيجة الصيغ.

```csharp
public void CalculateFormula(bool ignoreError)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ignoreError | منطقي | يشير إلى ما إذا كان يجب إخفاء الخطأ في حساب الصيغ. قد يكون الخطأ نتيجة دالة غير مدعومة، روابط خارجية، إلخ. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وخلاياها
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // وضع القيم في الصف الأول (A1:E1)
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(i + 1); // Values 1-5
            }

            // وضع القيم في الصف الثاني (A2:E2)
            for (int i = 0; i < 5; i++)
            {
                cells[1, i].PutValue((i + 1) * 10); // Values 10,20,30,40,50
            }

            // تعيين صيغة HLOOKUP مشتركة في الصف الرابع (A4:E4)
            cells[3, 0].SetSharedFormula("=HLOOKUP(A1,$A$1:$E$2,2,FALSE)", 1, 5);

            // حساب الصيغ دون حساب متكرر
            wb.CalculateFormula(false);

            // عرض النتائج
            Console.WriteLine("Formula calculation results:");
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Cell {((char)('A' + i))}4 value: {cells[3, i].StringValue}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions) {#calculateformula_1}

يتم حساب الصيغ في هذا المصنف.

```csharp
public void CalculateFormula(CalculationOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | CalculationOptions | خيارات الحساب |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithCalculationOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // إنشاء جدول وتعيين أسماء الأعمدة
            sheet.Cells["A1"].PutValue("A");
            sheet.Cells["B1"].PutValue("B");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(2);
            
            // تعيين الصيغ وحسابها
            Cells cells = sheet.Cells;
            cells["C1"].PutValue("InvalidColumn");
            cells["D1"].Formula = "=INDIRECT(\"A\"&ROW())";
            cells["E1"].Formula = "=IFERROR(INDIRECT(\"B\"&ROW()),\"OK\")";
            
            // حساب الصيغ مع خيارات
            wb.CalculateFormula(new CalculationOptions());
            
            // إخراج النتائج
            Console.WriteLine("D1 result: " + cells["D1"].StringValue);
            Console.WriteLine("E1 result: " + cells["E1"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


