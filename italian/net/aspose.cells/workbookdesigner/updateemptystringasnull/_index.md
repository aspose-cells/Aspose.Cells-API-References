---
title: "WorkbookDesigner.UpdateEmptyStringAsNull"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookDesigner. Se TRUE, verrà inserito Null se il valore è"
type: docs
url: /it/net/aspose.cells/workbookdesigner/updateemptystringasnull/
---
## WorkbookDesigner.UpdateEmptyStringAsNull property

Se TRUE, verrà inserito Null se il valore è "";

```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```

### Esempi

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
            // Crea un DataSet di esempio con stringhe vuote
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("Name");
            dt.Columns.Add("Price");
            dt.Rows.Add("Laptop", "");
            dt.Rows.Add("", "999.99");
            ds.Tables.Add(dt);

            // Crea una cartella di lavoro con i marker del designer
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&=$Products.Name");
            worksheet.Cells["B1"].PutValue("&=$Products.Price");

            // Inizializza WorkbookDesigner e imposta le proprietà
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.UpdateEmptyStringAsNull = true; // This is the key property being demonstrated
            
            // Imposta la fonte dati ed elabora
            designer.SetDataSource(ds.Tables["Products"]);
            designer.Process();

            // Verifica i risultati
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].StringValue); // Should show "Laptop"
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].StringValue); // Should show empty (null)
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


