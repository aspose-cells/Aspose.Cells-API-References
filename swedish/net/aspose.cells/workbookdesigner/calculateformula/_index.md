---
title: "WorkbookDesigner.CalculateFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner‑egenskap. Anger om formler ska beräknas"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/calculateformula/
---
## WorkbookDesigner.CalculateFormula property

Anger om formler ska beräknas.

```csharp
public bool CalculateFormula { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med en formel
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och formel
            worksheet.Cells["A1"].PutValue("Opportunity Name");
            worksheet.Cells["B1"].PutValue("Opportunity Amount");
            worksheet.Cells["A2"].PutValue("=Master.Opportunity_Name");
            worksheet.Cells["B2"].PutValue("=Master.Opportunity_Amount");
            worksheet.Cells["C2"].Formula = "=CONCATENATE(A2,B2)";

            // Skapa datakälla
            DataTable dt = new DataTable("Master");
            dt.Columns.Add("Opportunity_Name");
            dt.Columns.Add("Opportunity_Amount");
            DataRow dr = dt.NewRow();
            dr["Opportunity_Name"] = "Test Deal";
            dr["Opportunity_Amount"] = "$2500.00";
            dt.Rows.Add(dr);

            // Bearbeta designern med CalculateFormula aktiverat
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.SetDataSource(dt);
            designer.CalculateFormula = true; // This will calculate formulas after data binding
            designer.Process();

            // Skriv ut resultatet
            Console.WriteLine("Formula result: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


