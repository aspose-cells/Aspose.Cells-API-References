---
title: "WorkbookDesigner.RepeatFormulasWithSubtotal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà di WorkbookDesigner. Indica se le formule vengono ripetute con la riga di subtotale"
type: docs
url: /it/net/aspose.cells/workbookdesigner/repeatformulaswithsubtotal/
---
## WorkbookDesigner.RepeatFormulasWithSubtotal property

Indica se le formule vengono ripetute con la riga di subtotale.

```csharp
public bool RepeatFormulasWithSubtotal { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyRepeatFormulasWithSubtotalDemo
    {
        public static void Run()
        {
            // Crea un DataTable di esempio
            DataTable dt = new DataTable("products1");
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Quantity", typeof(int));
            
            // Aggiungi dati di esempio
            dt.Rows.Add(1, "Product A", 10.5m, 5);
            dt.Rows.Add(2, "Product B", 15.2m, 3);
            dt.Rows.Add(3, "Product C", 8.7m, 7);

            // Crea un nuovo workbook con una formula modello
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configura il modello con marker intelligenti e formula
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$UnitPrice");
            worksheet.Cells["D1"].PutValue("&=$Quantity");
            worksheet.Cells["E1"].PutValue("=SUM(C2:D2)"); // Formula to be repeated

            // Crea il designer e imposta RepeatFormulasWithSubtotal
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.RepeatFormulasWithSubtotal = true;
            designer.SetDataSource(dt);
            
            // Elabora il modello
            designer.Process();

            // Verifica che la formula sia stata ripetuta per ogni riga
            Console.WriteLine("Formula in E2: " + worksheet.Cells["E2"].Formula);
            Console.WriteLine("Formula in E3: " + worksheet.Cells["E3"].Formula);
            Console.WriteLine("Formula in E4: " + worksheet.Cells["E4"].Formula);

            // Salva il risultato
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


