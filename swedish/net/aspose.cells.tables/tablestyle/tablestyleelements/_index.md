---
title: "TableStyle.TableStyleElements"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TableStyle-egenskap. Hämtar alla element i tabellstilen"
type: docs
url: /sv/net/aspose.cells.tables/tablestyle/tablestyleelements/
---
## TableStyle.TableStyleElements property

Hämtar alla element i tabellstilen.

```csharp
public TableStyleElementCollection TableStyleElements { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStylePropertyTableStyleElementsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för tabellen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa en tabell
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTableStyleFirstColumn = true;

            // Hämta tabellstilen (använd befintlig stil istället för att skapa en ny)
            TableStyle style = workbook.Worksheets.TableStyles[0];

            // Modifiera tabellstilelement
            TableStyleElement wholeTableElement = style.TableStyleElements[TableStyleElementType.WholeTable];
            Style wholeTableStyle = wholeTableElement.GetElementStyle();
            wholeTableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            wholeTableStyle.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;

            // Applicera den modifierade stilen på tabellen
            table.TableStyleName = style.Name;

            // Spara arbetsboken
            workbook.Save("TableStyleElementsDemo.xlsx");
        }
    }
}
```

### Se även

* class [TableStyleElementCollection](../../tablestyleelementcollection/)
* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


