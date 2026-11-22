---
title: "Cell.IsErrorValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تتحقق مما إذا كانت قيمة هذه الخلية خطأ"
type: docs
url: /ar/net/aspose.cells/cell/iserrorvalue/
---
## Cell.IsErrorValue property

يتحقق مما إذا كانت قيمة هذه الخلية خطأ.

```csharp
public bool IsErrorValue { get; }
```

### ملاحظات

ينطبق أيضًا على خلية الصيغة للتحقق مما إذا كانت النتيجة المحسوبة خطأ.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsErrorValueDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // حدد صيغة ستؤدي إلى خطأ
            Cell cell = cells["A1"];
            cell.Formula = "=1/0"; // Division by zero error
            
            // حساب الصيغ
            workbook.CalculateFormula();

            // عرض خاصية IsErrorValue
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("IsErrorValue: " + cell.IsErrorValue);
            Console.WriteLine("Error type: " + cell.Value);

            // حدد قيمة صالحة
            Cell cell2 = cells["A2"];
            cell2.PutValue("Valid value");
            
            Console.WriteLine("\nCell A2 value: " + cell2.StringValue);
            Console.WriteLine("IsErrorValue: " + cell2.IsErrorValue);

            // تعيين خطأ SPILL (خطأ صيغة المصفوفة الديناميكية في Excel 365+)
            Cell cell3 = cells["A3"];
            cell3.SetDynamicArrayFormula("=A1:A10", new FormulaParseOptions(), true);
            
            Console.WriteLine("\nCell A3 value: " + cell3.StringValue);
            Console.WriteLine("IsErrorValue: " + cell3.IsErrorValue);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


