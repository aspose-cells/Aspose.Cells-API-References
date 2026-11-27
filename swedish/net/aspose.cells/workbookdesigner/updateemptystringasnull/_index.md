---
title: "WorkbookDesigner.UpdateEmptyStringAsNull"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner egenskap. Om TRUE Null kommer att infogas om värdet är"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/updateemptystringasnull/
---
## WorkbookDesigner.UpdateEmptyStringAsNull property

Om TRUE, infogas Null om värdet är "";

```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```

### Exempel

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
            // Skapa ett exempel-DataSet med tomma strängar
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("Name");
            dt.Columns.Add("Price");
            dt.Rows.Add("Laptop", "");
            dt.Rows.Add("", "999.99");
            ds.Tables.Add(dt);

            // Skapa en arbetsbok med designer-markörer
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&=$Products.Name");
            worksheet.Cells["B1"].PutValue("&=$Products.Price");

            // Initiera WorkbookDesigner och ange egenskaper
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.UpdateEmptyStringAsNull = true; // This is the key property being demonstrated
            
            // Ange datakälla och bearbeta
            designer.SetDataSource(ds.Tables["Products"]);
            designer.Process();

            // Verifiera resultat
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].StringValue); // Should show "Laptop"
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].StringValue); // Should show empty (null)
        }
    }
}
```

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


