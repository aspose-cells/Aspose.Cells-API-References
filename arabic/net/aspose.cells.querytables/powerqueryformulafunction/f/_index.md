---
title: "PowerQueryFormulaFunction.F"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormulaFunction. يحصل على ويضبط تعريف الدالة"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformulafunction/f/
---
## PowerQueryFormulaFunction.F property

يحصل على تعريف الدالة ويضبطه.

```csharp
public string F { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaFunctionPropertyFDemo
    {
        public static void Run()
        {
            // تحميل مصنف يحتوي على صيغ Power Query الموجودة
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى مجموعة صيغ Power Query
            PowerQueryFormulaCollection queryFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            // استرجاع صيغة دالة موجودة حسب الاسم
            PowerQueryFormula formula = queryFormulas["from_timestamp"];
            
            // تحويل إلى PowerQueryFormulaFunction للوصول إلى الخاصية F
            if (formula is PowerQueryFormulaFunction function)
            {
                // إظهار الحصول على الخاصية F
                Console.WriteLine("Original Function Definition: " + function.F);
                
                // إظهار تعيين الخاصية F
                function.F = "(x as number) as datetimezone => #datetimezone(1970,1,1,0,0,0,0,0) + #duration(0,0,0,x)";
                Console.WriteLine("Updated Function Definition: " + function.F);
            }
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


