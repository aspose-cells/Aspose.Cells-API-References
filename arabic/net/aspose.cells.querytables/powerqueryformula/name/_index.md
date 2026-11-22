---
title: "PowerQueryFormula.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormula. تحصل وتعيّن اسم صيغة استعلام الطاقة"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformula/name/
---
## PowerQueryFormula.Name property

يحصل على اسم صيغة استعلام Power Query ويضبطه.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تحميل ملف موجود يحتوي على صيغ Power Query
            workbook = new Workbook("example.xlsx");
            
            // الوصول إلى صيغ Power Query الموجودة
            if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
            {
                PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];
                
                // عرض استخدام خاصية Name
                Console.WriteLine("Original Power Query Formula Name: " + formula.Name);
                
                // تغيير الاسم
                formula.Name = "UpdatedSalesFilter";
                Console.WriteLine("Updated Power Query Formula Name: " + formula.Name);
                
                // احفظ المصنف
                workbook.Save("PowerQueryFormulaDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


