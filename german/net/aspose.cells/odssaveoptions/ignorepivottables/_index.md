---
title: "OdsSaveOptions.IgnorePivotTables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsSaveOptions‑Eigenschaft. Gibt an, ob Pivot-Tabellen gespeichert werden"
type: docs
url: /de/net/aspose.cells/odssaveoptions/ignorepivottables/
---
## OdsSaveOptions.IgnorePivotTables property

Gibt an, ob Pivot-Tabellen gespeichert werden.

```csharp
public bool IgnorePivotTables { get; set; }
```

### Hinweise

Die Pivot-Tabellen‑Funktion von OpenOffice verfügt über weniger Einstellungen im Vergleich zu Excel, sodass die Ergebnisse der Pivot‑Tabellen viele Unterschiede aufweisen. Manchmal ist es besser, diese Pivot‑Tabellen beim Speichern einer .ods‑Datei zu ignorieren.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsSaveOptionsPropertyIgnorePivotTablesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // Erstelle eine Pivot-Tabelle
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // OdsSaveOptions‑Instanz erstellen
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // Aktuellen Wert von IgnorePivotTables anzeigen
            Console.WriteLine("Current IgnorePivotTables value: " + saveOptions.IgnorePivotTables);

            // Auf Ignorieren von Pivot‑Tabellen beim Speichern setzen
            saveOptions.IgnorePivotTables = true;

            // Speichern mit ignorierten Pivot‑Tabellen
            workbook.Save("IgnorePivotTablesDemo_Ignored.ods", saveOptions);

            // Auf Einbeziehen von Pivot‑Tabellen beim Speichern setzen
            saveOptions.IgnorePivotTables = false;

            // Speichern mit einbezogenen Pivot‑Tabellen
            workbook.Save("IgnorePivotTablesDemo_Included.ods", saveOptions);
        }
    }
}
```

### Siehe auch

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


