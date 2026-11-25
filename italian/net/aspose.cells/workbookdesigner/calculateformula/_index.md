---
title: "WorkbookDesigner.CalculateFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookDesigner. Indica se le formule devono essere calcolate"
type: docs
url: /it/net/aspose.cells/workbookdesigner/calculateformula/
---
## WorkbookDesigner.CalculateFormula property

Indica se le formule devono essere calcolate.

```csharp
public bool CalculateFormula { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro di esempio con una formula
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e formula
            worksheet.Cells["A1"].PutValue("Opportunity Name");
            worksheet.Cells["B1"].PutValue("Opportunity Amount");
            worksheet.Cells["A2"].PutValue("=Master.Opportunity_Name");
            worksheet.Cells["B2"].PutValue("=Master.Opportunity_Amount");
            worksheet.Cells["C2"].Formula = "=CONCATENATE(A2,B2)";

            // Crea la fonte dati
            DataTable dt = new DataTable("Master");
            dt.Columns.Add("Opportunity_Name");
            dt.Columns.Add("Opportunity_Amount");
            DataRow dr = dt.NewRow();
            dr["Opportunity_Name"] = "Test Deal";
            dr["Opportunity_Amount"] = "$2500.00";
            dt.Rows.Add(dr);

            // Elabora il designer con CalculateFormula abilitato
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.SetDataSource(dt);
            designer.CalculateFormula = true; // This will calculate formulas after data binding
            designer.Process();

            // Restituisci il risultato
            Console.WriteLine("Formula result: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


