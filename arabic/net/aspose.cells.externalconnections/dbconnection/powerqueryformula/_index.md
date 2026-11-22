---
title: "DBConnection.PowerQueryFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DBConnection. يحصل على تعريف صيغة Power Query"
type: docs
url: /ar/net/aspose.cells.externalconnections/dbconnection/powerqueryformula/
---
## DBConnection.PowerQueryFormula property

يحصل على تعريف صيغة Power Query.

```csharp
public override PowerQueryFormula PowerQueryFormula { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.QueryTables;
    using System;

    public class DBConnectionPropertyPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى مجموعة الاتصالات الخارجية
                ExternalConnectionCollection connections = workbook.DataConnections;

                // العثور على أول DBConnection في المجموعة (إن وجد)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // الوصول إلى خاصية PowerQueryFormula (للقراءة فقط)
                    PowerQueryFormula powerQueryFormula = dbConn.PowerQueryFormula;

                    if (powerQueryFormula != null)
                    {
                        // عرض خصائص PowerQueryFormula
                        Console.WriteLine("PowerQueryFormula Type: " + powerQueryFormula.Type);
                        Console.WriteLine("PowerQueryFormula GroupName: " + powerQueryFormula.GroupName);
                        Console.WriteLine("PowerQueryFormula FormulaDefinition: " + powerQueryFormula.FormulaDefinition);
                        Console.WriteLine("PowerQueryFormula Name: " + powerQueryFormula.Name);
                        Console.WriteLine("PowerQueryFormula Description: " + powerQueryFormula.Description);

                        // إظهار كيفية الوصول إلى مجموعة PowerQueryFormulaItems
                        Console.WriteLine("Number of PowerQueryFormulaItems: " + powerQueryFormula.PowerQueryFormulaItems.Count);
                    }
                    else
                    {
                        Console.WriteLine("PowerQueryFormula is null for this connection.");
                    }
                }

                // احفظ المصنف
                workbook.Save("PowerQueryFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved as PowerQueryFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


