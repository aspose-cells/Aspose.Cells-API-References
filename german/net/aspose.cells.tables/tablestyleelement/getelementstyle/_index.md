---
title: "TableStyleElement.GetElementStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableStyleElement-Methode. Gibt den Elementstil zurück"
type: docs
url: /de/net/aspose.cells.tables/tablestyleelement/getelementstyle/
---
## TableStyleElement.GetElementStyle method

Liefert den Elementstil.

```csharp
public Style GetElementStyle()
```

### Rückgabewert

Gibt das [`Style`](../../../aspose.cells/style/)‑Objekt zurück.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Eine Tabelle erstellen
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Den Tabellenstil aus der Tabellestilsammlung des Arbeitsbuchs abrufen
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            TableStyle style = tableStyles[0];
            table.TableStyleName = style.Name;
            
            // Greifen Sie auf das gesamte Tabellestilelement zu
            TableStyleElement element = style.TableStyleElements[TableStyleElementType.WholeTable];
            
            // Den Elementstil abrufen
            Style tableStyle = element.GetElementStyle();
            
            // Die Stileigenschaften ändern
            tableStyle.Font.Name = "Arial";
            tableStyle.Font.Size = 12;
            tableStyle.Font.IsBold = true;
            tableStyle.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            tableStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            
            // Den geänderten Stil zurücksetzen
            element.SetElementStyle(tableStyle);
            
            // Speichere die Arbeitsmappe
            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../../aspose.cells/style/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


