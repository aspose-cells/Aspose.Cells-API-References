---
title: "WorkbookDesigner.RepeatFormulasWithSubtotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner-egenskap. Anger om formler ska upprepas med subtotalrad"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/repeatformulaswithsubtotal/
---
## WorkbookDesigner.RepeatFormulasWithSubtotal property

Anger om formler ska upprepas med en delrad.

```csharp
public bool RepeatFormulasWithSubtotal { get; set; }
```

### Exempel

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
            // Skapa en exempel-DataTable
            DataTable dt = new DataTable("products1");
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Quantity", typeof(int));
            
            // Lägg till exempeldata
            dt.Rows.Add(1, "Product A", 10.5m, 5);
            dt.Rows.Add(2, "Product B", 15.2m, 3);
            dt.Rows.Add(3, "Product C", 8.7m, 7);

            // Skapa en ny arbetsbok med en mallformel
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in mallen med smarta markörer och formel
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$UnitPrice");
            worksheet.Cells["D1"].PutValue("&=$Quantity");
            worksheet.Cells["E1"].PutValue("=SUM(C2:D2)"); // Formula to be repeated

            // Skapa designer och sätt RepeatFormulasWithSubtotal
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.RepeatFormulasWithSubtotal = true;
            designer.SetDataSource(dt);
            
            // Bearbeta mallen
            designer.Process();

            // Verifiera att formeln upprepades för varje rad
            Console.WriteLine("Formula in E2: " + worksheet.Cells["E2"].Formula);
            Console.WriteLine("Formula in E3: " + worksheet.Cells["E3"].Formula);
            Console.WriteLine("Formula in E4: " + worksheet.Cells["E4"].Formula);

            // Spara resultatet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


