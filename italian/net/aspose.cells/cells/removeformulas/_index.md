---
title: "Cells.RemoveFormulas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Rimuove tutte le formule e le sostituisce con il valore della formula"
type: docs
url: /it/net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

Rimuove tutte le formule e le sostituisce con il valore della formula.

```csharp
public void RemoveFormulas()
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveFormulasDemo
    {
        public static void Run()
        {
            // Crea un set di dati di esempio
            DataSet ds = new DataSet();

            // Crea e popola la tabella Master
            DataTable dtMaster = new DataTable("Master");
            dtMaster.Columns.Add("ACCOUNT", typeof(string));
            dtMaster.Columns.Add("ACCOUNT_CREATEDBY_NAME", typeof(string));
            dtMaster.Rows.Add("Test_Account", "Test_user");
            ds.Tables.Add(dtMaster);

            // Crea e popola la tabella OppLineItems
            DataTable lineItems = new DataTable("OppLineItems");
            lineItems.Columns.Add("Id", typeof(int));
            lineItems.Columns.Add("Name", typeof(string));
            lineItems.Columns.Add("SALESPRICE", typeof(int));
            lineItems.Rows.Add(1, "lineItem1", 10);
            lineItems.Rows.Add(2, "lineItem2", 20);
            ds.Tables.Add(lineItems);

            // Crea un nuovo workbook
            Workbook wkb = new Workbook();
            
            // Usa WorkbookDesigner per collegare i dati
            WorkbookDesigner designer = new WorkbookDesigner { Workbook = wkb };
            designer.SetDataSource(ds);
            designer.Process(false);

            // Aggiungi una formula per dimostrare la rimozione
            wkb.Worksheets[0].Cells["A10"].Formula = "=SUM(C2:C3)";
            
            // Calcola prima le formule
            wkb.CalculateFormula();

            // Rimuovi tutte le formule dal foglio di lavoro
            wkb.Worksheets[0].Cells.RemoveFormulas();

            // Salva la cartella di lavoro
            wkb.Save("output.xlsx");
            
            Console.WriteLine("Formulas removed and workbook saved successfully.");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


