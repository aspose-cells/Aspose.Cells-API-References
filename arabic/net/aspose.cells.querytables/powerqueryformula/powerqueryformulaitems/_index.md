---
title: "PowerQueryFormula.PowerQueryFormulaItems"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PowerQueryFormula. يحصل على جميع عناصر صيغة Power Query"
type: docs
url: /ar/net/aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/
---
## PowerQueryFormula.PowerQueryFormulaItems property

يحصل على جميع عناصر صيغة استعلام Power Query.

```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyPowerQueryFormulaItemsDemo
    {
        public static void Run()
        {
            // تحميل دفتر العمل المصدر
            Workbook workbook = new Workbook("example.xlsx");

            // الوصول إلى أول صيغة Power Query وعنصرها الأول
            PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            
            // تعديل قيمة العنصر (استبدال حرف محرك الأقراص)
            string modifiedValue = item.Value.Replace(@"C:\", @"D:\");
            item.Value = modifiedValue;

            // احفظ المصنف
            workbook.Save("modified_example.xlsx");

            // تحقق من التغيير
            Console.WriteLine("Original value modified to: " + modifiedValue);
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


