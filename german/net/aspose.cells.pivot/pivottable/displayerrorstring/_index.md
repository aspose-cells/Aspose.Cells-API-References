---
title: "PivotTable.DisplayErrorString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob der PivotTable-Bericht in Zellen, die Fehler enthalten, einen benutzerdefinierten Text anzeigt."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/displayerrorstring/
---
## PivotTable.DisplayErrorString property

Gibt an, ob der PivotTable-Bericht in Zellen, die Fehler enthalten, einen benutzerdefinierten Text anzeigt.

```csharp
public bool DisplayErrorString { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayErrorStringDemo
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
            cells["B5"].Value = 2500;

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Setze die DisplayErrorString-Eigenschaft und zeige ihre Verwendung.
            pivotTable.DisplayErrorString = true;
            pivotTable.ErrorString = "Custom Error";

            // Daten berechnen, um die Wirkung zu zeigen.
            pivotTable.CalculateData();

            Console.WriteLine("DisplayErrorString is set to: " + pivotTable.DisplayErrorString);
            Console.WriteLine("ErrorString is set to: " + pivotTable.ErrorString);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTablePropertyDisplayErrorStringDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


