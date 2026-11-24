---
title: "Worksheet.GetFreezedPanes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet method. Gibt die eingefrorenen Bereiche zurück."
type: docs
url: /de/net/aspose.cells/worksheet/getfreezedpanes/
---
## Worksheet.GetFreezedPanes method

Liest die eingefrorenen Bildschirmelemente.

```csharp
public bool GetFreezedPanes(out int row, out int column, out int freezedRows, 
    out int freezedColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32& | Zeilenindex. |
| column | Int32& | Spaltenindex. |
| freezedRows | Int32& | Anzahl der sichtbaren Zeilen im oberen Bereich, nicht mehr als Zeilenindex. |
| freezedColumns | Int32& | Anzahl der sichtbaren Spalten im linken Bereich, nicht mehr als Spaltenindex. |

### Rückgabewert

Gibt zurück, ob das Arbeitsblatt eingefroren ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodGetFreezedPanesWithInt32ParametersDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fenster bei Zelle C5 (Zeile 4, Spalte 2) einfrieren, mit 2 eingefrorenen Zeilen und 1 eingefrorener Spalte.
            worksheet.FreezePanes(4, 2, 2, 1);

            // Deklariere Variablen, um die Informationen zu den eingefrorenen Bereichen zu speichern.
            int row = 0;
            int column = 0;
            int freezedRows = 0;
            int freezedColumns = 0;

            try
            {
                // Rufe die GetFreezedPanes-Methode mit out-Parametern auf.
                bool hasFreeze = worksheet.GetFreezedPanes(out row, out column, out freezedRows, out freezedColumns);

                // Ergebnisse anzeigen
                Console.WriteLine("Worksheet has freeze panes: " + hasFreeze);
                if (hasFreeze)
                {
                    Console.WriteLine("Freeze position - Row: " + row + ", Column: " + column);
                    Console.WriteLine("Frozen rows: " + freezedRows + ", Frozen columns: " + freezedColumns);
                }

                // Speichere die Arbeitsmappe
                workbook.Save("WorksheetMethodGetFreezedPanesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFreezedPanes method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


