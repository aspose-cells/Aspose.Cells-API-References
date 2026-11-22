---
title: "ExternalConnection.PowerQueryFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحصل على تعريف صيغة power query"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/powerqueryformula/
---
## ExternalConnection.PowerQueryFormula property

يحصل على تعريف صيغة Power Query.

```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تحميل دفتر عمل موجود مع اتصالات بيانات لعرض PowerQueryFormula
            workbook = new Workbook("example.xlsx");
            
            // الوصول إلى اتصال موجود (مع افتراض أن دفتر العمل يحتوي على اتصال واحد على الأقل)
            if (workbook.DataConnections.Count > 0)
            {
                var connection = workbook.DataConnections[0];
                Console.WriteLine("Power Query Formula Demo:");
                Console.WriteLine($"Connection Name: {connection.Name}");
                
                // الوصول إلى خاصية PowerQueryFormula
                PowerQueryFormula powerQuery = connection.PowerQueryFormula;
                if (powerQuery != null)
                {
                    Console.WriteLine($"Formula Name: {powerQuery.Name}");
                    Console.WriteLine($"Formula Definition: {powerQuery.FormulaDefinition}");
                }
                else
                {
                    Console.WriteLine("No Power Query Formula found for this connection");
                }
            }
            else
            {
                Console.WriteLine("No data connections found in the workbook");
            }
            
            // احفظ المصنف
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


