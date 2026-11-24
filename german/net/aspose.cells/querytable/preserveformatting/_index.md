---
title: "QueryTable.PreserveFormatting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "QueryTable-Eigenschaft. Gibt das PreserveFormatting des Objekts zurück oder legt es fest"
type: docs
url: /de/net/aspose.cells/querytable/preserveformatting/
---
## QueryTable.PreserveFormatting property

Gibt die PreserveFormatting des Objekts zurück oder setzt sie.

```csharp
public bool PreserveFormatting { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten und Formatierung hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Formatierung auf den Datenbereich anwenden
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Stil auf jede Zelle im Bereich anwenden
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B1"].SetStyle(style);

            // Erstelle eine Abfrage‑Tabelle (simuliert, da die tatsächliche Erstellung eine externe Datenquelle erfordert)
            // In der Praxis würden Sie dies aus einer externen Verbindung erstellen
            QueryTable queryTable = worksheet.QueryTables[0];

            // Aktuellen PreserveFormatting-Wert anzeigen
            Console.WriteLine("Initial PreserveFormatting value: " + queryTable.PreserveFormatting);

            // Setze PreserveFormatting auf false (bestehende Formatierung wird beim Aktualisieren nicht beibehalten)
            queryTable.PreserveFormatting = false;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Simuliere das Aktualisieren der Abfrage‑Tabelle (würde normalerweise die Formatierung löschen, wenn PreserveFormatting false ist)
            // In einem realen Szenario würde dies geschehen, wenn die Abfrage‑Tabelle ihre Daten aktualisiert
            Console.WriteLine("After refresh with PreserveFormatting=false, formatting would be lost");

            // Setze PreserveFormatting wieder auf true
            queryTable.PreserveFormatting = true;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Simuliere das erneute Aktualisieren (würde jetzt die Formatierung beibehalten)
            Console.WriteLine("After refresh with PreserveFormatting=true, formatting is preserved");

            // Speichere die Arbeitsmappe
            workbook.Save("QueryTablePreserveFormattingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


