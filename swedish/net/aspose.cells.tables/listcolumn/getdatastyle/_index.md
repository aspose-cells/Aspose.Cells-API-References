---
title: "ListColumn.GetDataStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumn metod. Hämtar stilen för data i denna kolumn i tabellen"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/getdatastyle/
---
## ListColumn.GetDataStyle method

Hämtar stilen för data i denna kolumn i tabellen.

```csharp
public Style GetDataStyle()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetDataStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Skapa ett listobjekt (tabell)
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            
            // Hämta stil från den första listkolumnen
            Style style = table.ListColumns[0].GetDataStyle();
            
            // Modifiera stilen
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.Red;
            
            // Applicera den modifierade stilen tillbaka på kolumnen
            table.ListColumns[0].SetDataStyle(style);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../../aspose.cells/style/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


