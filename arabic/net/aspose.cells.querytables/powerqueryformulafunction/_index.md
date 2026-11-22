---
title: "الفئة PowerQueryFormulaFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.QueryTables.PowerQueryFormulaFunction. تمثل دالة Power Query"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulafunction/
---
## PowerQueryFormulaFunction class

يمثل دالة Power Query.

```csharp
public class PowerQueryFormulaFunction : PowerQueryFormula
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | يحصل ويضبط وصف صيغة استعلام الطاقة.(موروث من [`PowerQueryFormula`](../powerqueryformula/).) |
| [F](../../aspose.cells.querytables/powerqueryformulafunction/f/) { get; set; } | يحصل على تعريف الدالة ويضبطه. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | يحصل على تعريف صيغة استعلام الطاقة. (موروث من [`PowerQueryFormula`](../powerqueryformula/).) |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | يحصل على اسم المجموعة التي تحتوي على صيغة استعلام الطاقة.(موروث من [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | يحصل ويضبط اسم صيغة استعلام الطاقة.(موروث من [`PowerQueryFormula`](../powerqueryformula/).) |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | يحصل على جميع عناصر صيغة استعلام الطاقة.(موروث من [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulafunction/type/) { get; } | يحصل على نوع صيغة استعلام الطاقة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class QueryTablesClassPowerQueryFormulaFunctionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("source.xlsx");
            PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas["from_timestamp"];
            
            Console.WriteLine($"Name: {formula.Name}");
            Console.WriteLine($"Type: {formula.Type}");
            
            PowerQueryFormulaFunction function = (PowerQueryFormulaFunction)formula;
            Console.WriteLine($"Signature: {function.F}");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


