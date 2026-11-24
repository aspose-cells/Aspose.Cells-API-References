---
title: "PivotTable.NullString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable property. Gibt die Zeichenkette zurück, die in Zellen angezeigt wird, die Nullwerte enthalten, wenn die DisplayNullString‑Eigenschaft true ist. Der Standardwert ist eine leere Zeichenkette."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/nullstring/
---
## PivotTable.NullString property

Liest die Zeichenkette, die in Zellen angezeigt wird, die Nullwerte enthalten, wenn die Eigenschaft DisplayNullString wahr ist. Der Standardwert ist eine leere Zeichenkette.

```csharp
public string NullString { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyNullStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = null; // Null value
            cells["B5"].Value = 4000;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // NullString‑Eigenschaft und Anzeigeeinstellungen festlegen
            pivotTable.NullString = "(null)";
            pivotTable.DisplayNullString = true;

            // Pivot-Tabellendaten aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableNullStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


