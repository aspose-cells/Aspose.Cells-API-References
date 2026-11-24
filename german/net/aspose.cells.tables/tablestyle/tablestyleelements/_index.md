---
title: "TableStyle.TableStyleElements"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableStyle-Eigenschaft. Gibt alle Elemente des Tabellenstils zurück"
type: docs
url: /de/net/aspose.cells.tables/tablestyle/tablestyleelements/
---
## TableStyle.TableStyleElements property

Liest alle Elemente des Tabellenstils.

```csharp
public TableStyleElementCollection TableStyleElements { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die Tabelle erstellen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Eine Tabelle erstellen
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTableStyleFirstColumn = true;

            // Rufe den Tabellenstil ab (verwende einen vorhandenen Stil anstelle einen neuen zu erstellen)
            TableStyle style = workbook.Worksheets.TableStyles[0];

            // Tabellenstilelemente ändern
            TableStyleElement wholeTableElement = style.TableStyleElements[TableStyleElementType.WholeTable];
            Style wholeTableStyle = wholeTableElement.GetElementStyle();
            wholeTableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            wholeTableStyle.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;

            // Wende den modifizierten Stil auf die Tabelle an
            table.TableStyleName = style.Name;

            // Speichere die Arbeitsmappe
            workbook.Save("TableStyleElementsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TableStyleElementCollection](../../tablestyleelementcollection/)
* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


