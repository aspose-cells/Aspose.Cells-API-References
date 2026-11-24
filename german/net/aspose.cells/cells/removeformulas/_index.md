---
title: "Cells.RemoveFormulas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Entfernt alle Formeln und ersetzt sie durch den Wert der Formel"
type: docs
url: /de/net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

Entfernt alle Formeln und ersetzt sie durch den Wert der Formel.

```csharp
public void RemoveFormulas()
```

### Beispiele

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
            // Erstelle einen Beispiel-Datensatz
            DataSet ds = new DataSet();

            // Erstelle und fülle die Master-Tabelle
            DataTable dtMaster = new DataTable("Master");
            dtMaster.Columns.Add("ACCOUNT", typeof(string));
            dtMaster.Columns.Add("ACCOUNT_CREATEDBY_NAME", typeof(string));
            dtMaster.Rows.Add("Test_Account", "Test_user");
            ds.Tables.Add(dtMaster);

            // Erstelle und fülle die OppLineItems-Tabelle
            DataTable lineItems = new DataTable("OppLineItems");
            lineItems.Columns.Add("Id", typeof(int));
            lineItems.Columns.Add("Name", typeof(string));
            lineItems.Columns.Add("SALESPRICE", typeof(int));
            lineItems.Rows.Add(1, "lineItem1", 10);
            lineItems.Rows.Add(2, "lineItem2", 20);
            ds.Tables.Add(lineItems);

            // Erstelle ein neues Arbeitsbuch
            Workbook wkb = new Workbook();
            
            // Verwende WorkbookDesigner, um Daten zu binden
            WorkbookDesigner designer = new WorkbookDesigner { Workbook = wkb };
            designer.SetDataSource(ds);
            designer.Process(false);

            // Füge eine Formel hinzu, um die Entfernung zu demonstrieren
            wkb.Worksheets[0].Cells["A10"].Formula = "=SUM(C2:C3)";
            
            // Formeln zuerst berechnen
            wkb.CalculateFormula();

            // Alle Formeln aus dem Arbeitsblatt entfernen
            wkb.Worksheets[0].Cells.RemoveFormulas();

            // Speichere die Arbeitsmappe
            wkb.Save("output.xlsx");
            
            Console.WriteLine("Formulas removed and workbook saved successfully.");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


