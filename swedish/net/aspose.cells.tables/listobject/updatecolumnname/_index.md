---
title: "ListObject.UpdateColumnName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject metod. Uppdaterar alla listkolumners namn till cellerna i tabellen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/updatecolumnname/
---
## ListObject.UpdateColumnName method

Uppdaterar alla listkolumners namn till cellerna i tabellen.

```csharp
public void UpdateColumnName()
```

### Anmärkningar

Värdet på cellerna i rubrikraden i tabellen måste vara samma som namnet på ListColumn; Cell.PutValue ändrar inte automatiskt namnet på ListColumn av prestandaskäl.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectMethodUpdateColumnNameDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Skapa ett tabell/list-objekt
            var listObject = ws.ListObjects[ws.ListObjects.Add(3, 3, 6, 6, true)];
            
            // Fyll i lite data i tabellen
            for (int r = 0; r < 3; r++)
            {
                for (int c = 0; c < 3; c++)
                {
                    if (c > 0)
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue(r + c);
                    else
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue("");
                }
            }

            // Uppdatera kolumnnamn (kommer att sätta standardnamn som Column1, Column2 osv.)
            listObject.UpdateColumnName();

            // Spara arbetsboken
            wb.Save("output.xlsx");

            // Verifiera att kolumnnamnet uppdaterades
            Console.WriteLine("First column name: " + ws.Cells[listObject.StartRow, listObject.StartColumn].StringValue);
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


