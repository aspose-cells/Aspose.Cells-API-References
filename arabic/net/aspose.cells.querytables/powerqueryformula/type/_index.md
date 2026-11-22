---
title: "PowerQueryFormula.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormula. تحصل على نوع صيغة استعلام الطاقة هذه"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformula/type/
---
## PowerQueryFormula.Type property

يحصل على نوع صيغة استعلام Power Query هذه.

```csharp
public virtual PowerQueryFormulaType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على الصيغ الموجودة (لا توجد في المصنف الجديد) لتوضيح خاصية Type
            var formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // في سيناريو واقعي مع الصيغ الموجودة، كنا سنفحص أنواعها
            Console.WriteLine("Power Query Formula Types:");
            
            // هذا يوضح فحص خاصية Type
            foreach (PowerQueryFormula formula in formulas)
            {
                Console.WriteLine($"- {formula.Name}: {formula.Type}");
            }

            // لأغراض العرض، أضف مخرجات عندما لا توجد صيغ
            if (formulas.Count == 0)
            {
                Console.WriteLine("No power query formulas found in the workbook.");
                Console.WriteLine("Example formula types would be:");
                Console.WriteLine("- Function: " + PowerQueryFormulaType.Function);
                Console.WriteLine("- Parameter: " + PowerQueryFormulaType.Parameter);
                Console.WriteLine("- Formula: " + PowerQueryFormulaType.Formula);
            }

            // احفظ المصنف
            workbook.Save("PowerQueryFormulaTypes.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


