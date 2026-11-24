---
title: "QueryTable.AdjustColumnWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "QueryTable-Eigenschaft. Gibt das AdjustColumnWidth-Attribut des Objekts zurück oder setzt es"
type: docs
url: /de/net/aspose.cells/querytable/adjustcolumnwidth/
---
## QueryTable.AdjustColumnWidth property

Gibt die AdjustColumnWidth des Objekts zurück oder setzt sie.

```csharp
public bool AdjustColumnWidth { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyAdjustColumnWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten mit unterschiedlichen Spaltenbreiten hinzu
            worksheet.Cells["A1"].PutValue("Narrow Column");
            worksheet.Cells["B1"].PutValue("Wide Column Data");
            worksheet.Cells["A2"].PutValue("Short");
            worksheet.Cells["B2"].PutValue("This is some very long text that should demonstrate column width adjustment");

            // Setzen Sie Spaltenbreiten manuell
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 10); // Initially narrow for wide data

            // Erstelle eine Abfrage‑Tabelle (simuliert, da die tatsächliche Erstellung eine externe Datenquelle erfordert)
            QueryTable queryTable = worksheet.QueryTables[0];

            // Zeige den aktuellen AdjustColumnWidth‑Wert an
            Console.WriteLine("Initial AdjustColumnWidth value: " + queryTable.AdjustColumnWidth);

            // Setze AdjustColumnWidth auf true und zeige die Wirkung
            queryTable.AdjustColumnWidth = true;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);
            Console.WriteLine("After setting to true, columns would auto-adjust to fit content during refresh");

            // Simuliere das Aktualisieren der Abfrage‑Tabelle (würde normalerweise Spaltenbreiten anpassen)
            // In einem realen Szenario würde dies geschehen, wenn die Abfrage‑Tabelle ihre Daten aktualisiert
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=true:");
            Console.WriteLine("Column A width: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width: " + worksheet.Cells.GetColumnWidth(1));

            // Setze AdjustColumnWidth auf false und zeige die Wirkung
            queryTable.AdjustColumnWidth = false;
            Console.WriteLine("AdjustColumnWidth set to: " + queryTable.AdjustColumnWidth);

            // Simuliere das erneute Aktualisieren (würde jetzt die ursprünglichen Spaltenbreiten beibehalten)
            Console.WriteLine("Column widths after refresh with AdjustColumnWidth=false:");
            Console.WriteLine("Column A width remains: " + worksheet.Cells.GetColumnWidth(0));
            Console.WriteLine("Column B width remains: " + worksheet.Cells.GetColumnWidth(1));

            // Speichere die Arbeitsmappe
            workbook.Save("QueryTableAdjustColumnWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


