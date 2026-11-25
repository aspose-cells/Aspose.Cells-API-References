---
title: "Workbook.GetNamedStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Ottiene lo stile nominato nel pool di stili"
type: docs
url: /it/net/aspose.cells/workbook/getnamedstyle/
---
## Workbook.GetNamedStyle method

Ottiene lo stile denominato nel pool di stili.

```csharp
public Style GetNamedStyle(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | nome dello stile |

### Valore di ritorno

stile nominato, potrebbe essere null.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetNamedStyleWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni stili nominati
            Style style1 = workbook.CreateStyle();
            style1.Name = "Number7";
            style1.Custom = "#,##0.00";
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "Center";
            style2.HorizontalAlignment = TextAlignmentType.Center;
            
            // Crea dati di esempio
            DataTable dt = new DataTable();
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("Quantity", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Discount", typeof(float));
            
            dt.Rows.Add(1, "Product A", 10, 19.99m, 0.1f);
            dt.Rows.Add(2, "Product B", 5, 29.99m, 0.15f);
            
            // Ottieni foglio di lavoro e celle
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Ottieni stili denominati
            Style numberStyle = workbook.GetNamedStyle("Number7");
            Style centerStyle = workbook.GetNamedStyle("Center");
            
            // Applica stili ai dati
            for(int i = 0; i < dt.Rows.Count; i++)
            {
                cells[i, 0].PutValue((int)dt.Rows[i]["ProductID"]);
                cells[i, 0].SetStyle(centerStyle);
                
                cells[i, 1].PutValue((string)dt.Rows[i]["ProductName"]);
                
                cells[i, 3].PutValue((decimal)dt.Rows[i]["UnitPrice"]);
                cells[i, 3].SetStyle(numberStyle);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("GetNamedStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


