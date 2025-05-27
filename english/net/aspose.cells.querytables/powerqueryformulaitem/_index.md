---
title: Class PowerQueryFormulaItem
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormulaItem class. Represents the item of the power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

Represents the item of the power query formula.

```csharp
public class PowerQueryFormulaItem
```

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | Gets the name of the item. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | Gets the value of the item. |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class QueryTablesClassPowerQueryFormulaItemDemo
    {
        public static void Run()
        {
            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample Power Query data
            worksheet.Cells["A1"].PutValue("Sample Power Query Data");
            
            // Access Power Query formulas (note: actual Power Query requires Excel file with existing queries)
            PowerQueryFormulaCollection PQFcoll = workbook.DataMashup.PowerQueryFormulas;
            
            // This is just a demo - normally you would work with existing queries
            Console.WriteLine("Number of Power Query Formulas: {0}", PQFcoll.Count);
            
            // Save the workbook
            workbook.Save("PowerQueryDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


