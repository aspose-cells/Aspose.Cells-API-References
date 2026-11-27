---
title: "WorkbookDesigner.UpdateReference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner egenskap. Anger om referenser i andra kalkylblad kommer att uppdateras"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/updatereference/
---
## WorkbookDesigner.UpdateReference property

Anger om referenser i andra kalkylblad kommer att uppdateras.

```csharp
public bool UpdateReference { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Skapa ett exempel på dataset
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ID", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Columns.Add("Price", typeof(decimal));
            
            dt.Rows.Add(1, "Product A", 19.99);
            dt.Rows.Add(2, "Product B", 29.99);
            dt.Rows.Add(3, "Product C", 39.99);
            
            ds.Tables.Add(dt);

            // Skapa en arbetsbokdesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Ange UpdateReference-egenskapen till true
            designer.UpdateReference = true;
            
            // Skapa en ny arbetsbok med en mall
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till smarta markörer
            worksheet.Cells["A1"].PutValue("&=Products.ID");
            worksheet.Cells["B1"].PutValue("&=Products.Name");
            worksheet.Cells["C1"].PutValue("&=Products.Price");
            
            designer.Workbook = workbook;
            designer.SetDataSource("Products", dt);
            
            // Bearbeta designern
            designer.Process();
            
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


