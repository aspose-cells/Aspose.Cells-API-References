---
title: "WorkbookDesigner.CalculateFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner‑Eigenschaft. Gibt an, ob Formeln berechnet werden sollen"
type: docs
url: /de/net/aspose.cells/workbookdesigner/calculateformula/
---
## WorkbookDesigner.CalculateFormula property

Gibt an, ob Formeln berechnet werden sollen.

```csharp
public bool CalculateFormula { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine Beispielarbeitsmappe mit einer Formel
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und Formel hinzufügen
            worksheet.Cells["A1"].PutValue("Opportunity Name");
            worksheet.Cells["B1"].PutValue("Opportunity Amount");
            worksheet.Cells["A2"].PutValue("=Master.Opportunity_Name");
            worksheet.Cells["B2"].PutValue("=Master.Opportunity_Amount");
            worksheet.Cells["C2"].Formula = "=CONCATENATE(A2,B2)";

            // Datenquelle erstellen
            DataTable dt = new DataTable("Master");
            dt.Columns.Add("Opportunity_Name");
            dt.Columns.Add("Opportunity_Amount");
            DataRow dr = dt.NewRow();
            dr["Opportunity_Name"] = "Test Deal";
            dr["Opportunity_Amount"] = "$2500.00";
            dt.Rows.Add(dr);

            // Verarbeiten Sie den Designer mit aktivierter CalculateFormula‑Option
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.SetDataSource(dt);
            designer.CalculateFormula = true; // This will calculate formulas after data binding
            designer.Process();

            // Gib das Ergebnis aus
            Console.WriteLine("Formula result: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


