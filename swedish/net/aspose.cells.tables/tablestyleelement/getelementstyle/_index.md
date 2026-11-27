---
title: "TableStyleElement.GetElementStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TableStyleElement-metod. Hämtar elementstilen"
type: docs
url: /sv/net/aspose.cells.tables/tablestyleelement/getelementstyle/
---
## TableStyleElement.GetElementStyle method

Hämtar elementstilen.

```csharp
public Style GetElementStyle()
```

### Returvärde

Returnerar [`Style`](../../../aspose.cells/style/) objektet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementMethodGetElementStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Skapa en tabell
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Hämta tabellstilen från arbetsbokens tabellstilsamling
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            TableStyle style = tableStyles[0];
            table.TableStyleName = style.Name;
            
            // Åtkomst till hela tabellstilelementet
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.WholeTable];
            
            // Hämta elementstilen
            Style tableStyle = element.GetElementStyle();
            
            // Ändra stilens egenskaper
            tableStyle.Font.Name = "Arial";
            tableStyle.Font.Size = 12;
            tableStyle.Font.IsBold = true;
            tableStyle.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            
            // Ställ in den ändrade stilen tillbaka
            element.SetElementStyle(tableStyle);
            
            // Spara arbetsboken
            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../../aspose.cells/style/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


