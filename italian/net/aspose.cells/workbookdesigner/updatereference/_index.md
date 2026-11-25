---
title: "WorkbookDesigner.UpdateReference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookDesigner. Indica se i riferimenti in altri fogli di lavoro saranno aggiornati"
type: docs
url: /it/net/aspose.cells/workbookdesigner/updatereference/
---
## WorkbookDesigner.UpdateReference property

Indica se i riferimenti in altri fogli di lavoro verranno aggiornati.

```csharp
public bool UpdateReference { get; set; }
```

### Esempi

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
            // Crea un set di dati di esempio
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ID", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Columns.Add("Price", typeof(decimal));
            
            dt.Rows.Add(1, "Product A", 19.99);
            dt.Rows.Add(2, "Product B", 29.99);
            dt.Rows.Add(3, "Product C", 39.99);
            
            ds.Tables.Add(dt);

            // Crea un designer di cartella di lavoro
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Imposta la proprietà UpdateReference su true
            designer.UpdateReference = true;
            
            // Crea una nuova cartella di lavoro con un modello
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi smart markers
            worksheet.Cells["A1"].PutValue("&=Products.ID");
            worksheet.Cells["B1"].PutValue("&=Products.Name");
            worksheet.Cells["C1"].PutValue("&=Products.Price");
            
            designer.Workbook = workbook;
            designer.SetDataSource("Products", dt);
            
            // Elabora il designer
            designer.Process();
            
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


