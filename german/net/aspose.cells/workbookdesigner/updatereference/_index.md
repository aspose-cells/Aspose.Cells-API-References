---
title: "WorkbookDesigner.UpdateReference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner-Eigenschaft. Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden"
type: docs
url: /de/net/aspose.cells/workbookdesigner/updatereference/
---
## WorkbookDesigner.UpdateReference property

Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden.

```csharp
public bool UpdateReference { get; set; }
```

### Beispiele

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
            // Erstelle einen Beispiel-Datensatz
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ID", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Columns.Add("Price", typeof(decimal));
            
            dt.Rows.Add(1, "Product A", 19.99);
            dt.Rows.Add(2, "Product B", 29.99);
            dt.Rows.Add(3, "Product C", 39.99);
            
            ds.Tables.Add(dt);

            // Erstelle einen WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Setze die UpdateReference-Eigenschaft auf true
            designer.UpdateReference = true;
            
            // Erstelle eine neue Arbeitsmappe mit einer Vorlage
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Smartmarker hinzu
            worksheet.Cells["A1"].PutValue("&=Products.ID");
            worksheet.Cells["B1"].PutValue("&=Products.Name");
            worksheet.Cells["C1"].PutValue("&=Products.Price");
            
            designer.Workbook = workbook;
            designer.SetDataSource("Products", dt);
            
            // Verarbeite den Designer
            designer.Process();
            
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


