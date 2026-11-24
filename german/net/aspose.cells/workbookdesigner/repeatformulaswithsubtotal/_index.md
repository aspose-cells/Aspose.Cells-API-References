---
title: "WorkbookDesigner.RepeatFormulasWithSubtotal"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner‑Eigenschaft. Gibt an, ob Formeln mit Zwischensummen‑Zeile wiederholt werden"
type: docs
url: /de/net/aspose.cells/workbookdesigner/repeatformulaswithsubtotal/
---
## WorkbookDesigner.RepeatFormulasWithSubtotal property

Gibt an, ob Formeln mit Zwischensummenzeile wiederholt werden.

```csharp
public bool RepeatFormulasWithSubtotal { get; set; }
```

### Beispiele

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
            // Erstelle ein Beispiel-DataTable
            DataTable dt = new DataTable("products1");
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Quantity", typeof(int));
            
            // Fügen Sie Beispieldaten hinzu
            dt.Rows.Add(1, "Product A", 10.5m, 5);
            dt.Rows.Add(2, "Product B", 15.2m, 3);
            dt.Rows.Add(3, "Product C", 8.7m, 7);

            // Erstellen Sie eine neue Arbeitsmappe mit einer Vorlagenformel
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Richten Sie die Vorlage mit Smart‑Markern und Formel ein
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$UnitPrice");
            worksheet.Cells["D1"].PutValue("&=$Quantity");
            worksheet.Cells["E1"].PutValue("=SUM(C2:D2)"); // Formula to be repeated

            // Erstellen Sie den Designer und setzen Sie RepeatFormulasWithSubtotal
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.RepeatFormulasWithSubtotal = true;
            designer.SetDataSource(dt);
            
            // Verarbeiten Sie die Vorlage
            designer.Process();

            // Überprüfen Sie, ob die Formel für jede Zeile wiederholt wurde
            Console.WriteLine("Formula in E2: " + worksheet.Cells["E2"].Formula);
            Console.WriteLine("Formula in E3: " + worksheet.Cells["E3"].Formula);
            Console.WriteLine("Formula in E4: " + worksheet.Cells["E4"].Formula);

            // Ergebnis speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


