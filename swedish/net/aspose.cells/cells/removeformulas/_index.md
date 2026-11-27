---
title: "Cells.RemoveFormulas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Tar bort alla formler och ersätter dem med formelns värde"
type: docs
url: /sv/net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

Tar bort alla formler och ersätter dem med formelns värde.

```csharp
public void RemoveFormulas()
```

### Exempel

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
            // Skapa ett exempel på dataset
            DataSet ds = new DataSet();

            // Skapa och fyll i Master-tabell
            DataTable dtMaster = new DataTable("Master");
            dtMaster.Columns.Add("ACCOUNT", typeof(string));
            dtMaster.Columns.Add("ACCOUNT_CREATEDBY_NAME", typeof(string));
            dtMaster.Rows.Add("Test_Account", "Test_user");
            ds.Tables.Add(dtMaster);

            // Skapa och fyll i OppLineItems-tabell
            DataTable lineItems = new DataTable("OppLineItems");
            lineItems.Columns.Add("Id", typeof(int));
            lineItems.Columns.Add("Name", typeof(string));
            lineItems.Columns.Add("SALESPRICE", typeof(int));
            lineItems.Rows.Add(1, "lineItem1", 10);
            lineItems.Rows.Add(2, "lineItem2", 20);
            ds.Tables.Add(lineItems);

            // Skapa en ny arbetsbok
            Workbook wkb = new Workbook();
            
            // Använd WorkbookDesigner för att binda data
            WorkbookDesigner designer = new WorkbookDesigner { Workbook = wkb };
            designer.SetDataSource(ds);
            designer.Process(false);

            // Lägg till en formel för att demonstrera borttagning
            wkb.Worksheets[0].Cells["A10"].Formula = "=SUM(C2:C3)";
            
            // Beräkna formler först
            wkb.CalculateFormula();

            // Ta bort alla formler från arbetsbladet
            wkb.Worksheets[0].Cells.RemoveFormulas();

            // Spara arbetsboken
            wkb.Save("output.xlsx");
            
            Console.WriteLine("Formulas removed and workbook saved successfully.");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


