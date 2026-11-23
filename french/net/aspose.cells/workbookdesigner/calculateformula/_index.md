---
title: "WorkbookDesigner.CalculateFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookDesigner. Indique si les formules doivent être calculées"
type: docs
url: /fr/net/aspose.cells/workbookdesigner/calculateformula/
---
## WorkbookDesigner.CalculateFormula property

Indique si les formules doivent être calculées.

```csharp
public bool CalculateFormula { get; set; }
```

### Exemples

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
            // Créer un classeur d'exemple avec une formule
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple et une formule
            worksheet.Cells["A1"].PutValue("Opportunity Name");
            worksheet.Cells["B1"].PutValue("Opportunity Amount");
            worksheet.Cells["A2"].PutValue("=Master.Opportunity_Name");
            worksheet.Cells["B2"].PutValue("=Master.Opportunity_Amount");
            worksheet.Cells["C2"].Formula = "=CONCATENATE(A2,B2)";

            // Créer une source de données
            DataTable dt = new DataTable("Master");
            dt.Columns.Add("Opportunity_Name");
            dt.Columns.Add("Opportunity_Amount");
            DataRow dr = dt.NewRow();
            dr["Opportunity_Name"] = "Test Deal";
            dr["Opportunity_Amount"] = "$2500.00";
            dt.Rows.Add(dr);

            // Traiter le concepteur avec CalculateFormula activé
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.SetDataSource(dt);
            designer.CalculateFormula = true; // This will calculate formulas after data binding
            designer.Process();

            // Afficher le résultat
            Console.WriteLine("Formula result: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### Voir aussi

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


