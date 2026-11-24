---
title: "PivotTable.ErrorString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt die Zeichenkette zurück, die in Zellen angezeigt wird, die Fehler enthalten, wenn die Eigenschaft DisplayErrorString true ist. Der Standardwert ist eine leere Zeichenkette."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/errorstring/
---
## PivotTable.ErrorString property

Liest den Text, der in Zellen mit Fehlern angezeigt wird, wenn die Eigenschaft DisplayErrorString true ist. Der Standardwert ist ein leerer String.

```csharp
public string ErrorString { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyErrorStringDemo
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
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 1800;

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // ErrorString-Eigenschaft setzen
            pivotTable.ErrorString = "Custom Error";
            pivotTable.DisplayErrorString = true;

            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Daten berechnen und PivotTable aktualisieren
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableErrorStringDemo.xlsx");

            Console.WriteLine("PivotTable with ErrorString property set successfully.");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


