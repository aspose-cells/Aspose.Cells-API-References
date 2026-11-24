---
title: "WorkbookDesigner.UpdateEmptyStringAsNull"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner‑Eigenschaft. Wenn TRUE, wird Null eingefügt, wenn der Wert ist"
type: docs
url: /de/net/aspose.cells/workbookdesigner/updateemptystringasnull/
---
## WorkbookDesigner.UpdateEmptyStringAsNull property

Wenn TRUE, wird Null eingefügt, wenn der Wert "" ist;

```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyUpdateEmptyStringAsNullDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispiel-DataSet mit leeren Zeichenketten
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("Name");
            dt.Columns.Add("Price");
            dt.Rows.Add("Laptop", "");
            dt.Rows.Add("", "999.99");
            ds.Tables.Add(dt);

            // Erstelle eine Arbeitsmappe mit Designer-Markern
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&=$Products.Name");
            worksheet.Cells["B1"].PutValue("&=$Products.Price");

            // Initialisiere WorkbookDesigner und setze Eigenschaften
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.UpdateEmptyStringAsNull = true; // This is the key property being demonstrated
            
            // Setze Datenquelle und verarbeite
            designer.SetDataSource(ds.Tables["Products"]);
            designer.Process();

            // Ergebnis überprüfen
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].StringValue); // Should show "Laptop"
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].StringValue); // Should show empty (null)
        }
    }
}
```

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


