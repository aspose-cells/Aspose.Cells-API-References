---
title: "Workbook.GetNamedStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Hämtar den namngivna stilen i stilpoolen"
type: docs
url: /sv/net/aspose.cells/workbook/getnamedstyle/
---
## Workbook.GetNamedStyle method

Hämtar den namngivna stilen i stilpoolen.

```csharp
public Style GetNamedStyle(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | namn på stilen |

### Returvärde

namngiven stil, kan vara null.

### Exempel

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
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några namngivna stilar
            Style style1 = workbook.CreateStyle();
            style1.Name = "Number7";
            style1.Custom = "#,##0.00";
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "Center";
            style2.HorizontalAlignment = TextAlignmentType.Center;
            
            // Skapa exempeldata
            DataTable dt = new DataTable();
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("Quantity", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Discount", typeof(float));
            
            dt.Rows.Add(1, "Product A", 10, 19.99m, 0.1f);
            dt.Rows.Add(2, "Product B", 5, 29.99m, 0.15f);
            
            // Hämta kalkylblad och celler
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Hämta namngivna stilar
            Style numberStyle = workbook.GetNamedStyle("Number7");
            Style centerStyle = workbook.GetNamedStyle("Center");
            
            // Applicera stilar på data
            for(int i = 0; i < dt.Rows.Count; i++)
            {
                cells[i, 0].PutValue((int)dt.Rows[i]["ProductID"]);
                cells[i, 0].SetStyle(centerStyle);
                
                cells[i, 1].PutValue((string)dt.Rows[i]["ProductName"]);
                
                cells[i, 3].PutValue((decimal)dt.Rows[i]["UnitPrice"]);
                cells[i, 3].SetStyle(numberStyle);
            }
            
            // Spara arbetsboken
            workbook.Save("GetNamedStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


