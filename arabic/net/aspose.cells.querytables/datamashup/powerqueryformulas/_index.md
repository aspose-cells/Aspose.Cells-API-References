---
title: "DataMashup.PowerQueryFormulas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataMashup. يحصل على جميع صيغ Power Query"
type: docs
url: /ar/net/aspose.cells.querytables/datamashup/powerqueryformulas/
---
## DataMashup.PowerQueryFormulas property

يحصل على جميع صيغ Power Query.

```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulasDemo
    {
        public static void Run()
        {
            // تحميل دفتر العمل بصيغ Power Query
            Workbook workbook = new Workbook("source.xlsx");
            
            // الحصول على كائن DataMashup
            DataMashup mashupData = workbook.DataMashup;
            
            // تحقق مما إذا كان هناك أي صيغ Power Query
            if (mashupData != null && mashupData.PowerQueryFormulas != null)
            {
                Console.WriteLine("Power Query Formulas Found:");
                
                // تكرار عبر كل صيغة Power Query
                foreach (PowerQueryFormula formula in mashupData.PowerQueryFormulas)
                {
                    Console.WriteLine("Formula Definition:");
                    Console.WriteLine(formula.FormulaDefinition);
                    Console.WriteLine("----------------------");
                }
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


