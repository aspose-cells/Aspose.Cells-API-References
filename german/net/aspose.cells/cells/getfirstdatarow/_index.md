---
title: "Cells.GetFirstDataRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Ruft den Index der ersten Zeile einer Zelle ab, die Daten in der angegebenen Spalte enthält"
type: docs
url: /de/net/aspose.cells/cells/getfirstdatarow/
---
## Cells.GetFirstDataRow method

Gibt den Index der ersten Zeile der Zelle zurück, die Daten in der angegebenen Spalte enthält.

```csharp
public int GetFirstDataRow(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex. |

### Rückgabewert

Erster Zeilenindex.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetFirstDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten hinzu, um die Methode zu demonstrieren
            worksheet.Cells["A1"].Value = "Header";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["A3"].Value = "Data2";
            worksheet.Cells["B5"].Value = "Data3";
            worksheet.Cells["C7"].Value = "Data4";

            try
            {
                // Rufe die Cells-Sammlung aus dem Arbeitsblatt ab
                Cells cells = worksheet.Cells;

                // Rufen Sie GetFirstDataRow für Spalte A (Index 0) auf
                int firstDataRowA = cells.GetFirstDataRow(0);
                Console.WriteLine($"First data row in column A: {firstDataRowA}");

                // Rufen Sie GetFirstDataRow für Spalte B (Index 1) auf
                int firstDataRowB = cells.GetFirstDataRow(1);
                Console.WriteLine($"First data row in column B: {firstDataRowB}");

                // Rufen Sie GetFirstDataRow für Spalte C (Index 2) auf
                int firstDataRowC = cells.GetFirstDataRow(2);
                Console.WriteLine($"First data row in column C: {firstDataRowC}");

                // Speichere die Arbeitsmappe
                workbook.Save("GetFirstDataRowDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


