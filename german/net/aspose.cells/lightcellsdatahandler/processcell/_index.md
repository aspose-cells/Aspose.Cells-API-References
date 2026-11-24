---
title: "LightCellsDataHandler.ProcessCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LightCellsDataHandler-Methode. Beginnt mit der Verarbeitung einer Zelle"
type: docs
url: /de/net/aspose.cells/lightcellsdatahandler/processcell/
---
## LightCellsDataHandler.ProcessCell method

Beginnt mit der Verarbeitung einer Zelle.

```csharp
public bool ProcessCell(Cell cell)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zelle | Zelle | Zellenobjekt, das gerade verarbeitet wird |

### Rückgabewert

Ob diese Zelle im Zellenmodell des aktuellen Arbeitsblatts behalten werden muss. In der Regel sollte dies false sein, damit alle Zellen nach ihrer Verarbeitung nicht im Speicher gehalten werden und Speicher gespart wird. Für spezielle Zwecke, z. B. wenn der Benutzer später nach der Verarbeitung der gesamten Arbeitsmappe auf einige Zellen zugreifen muss, kann der Benutzer diese Methode true zurückgeben, um diese speziellen Zellen im Cells‑Modell zu behalten und später über APIs wie Cells[row, column] darauf zuzugreifen. Das Behalten von Zellen­daten im Cells‑Modell erfordert jedoch mehr Speicher, und wenn alle Zellen behalten werden, wird das Lesen der Vorlagendatei im LightCells‑Modus dasselbe wie das Lesen im normalen Modus.

### Hinweise

Sie wird aufgerufen, nachdem die Daten einer Zelle gelesen wurden.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodProcessCellWithCellDemo
    {
        public static void Run()
        {
            try
            {
                // Temporäre Datendatei erstellen
                File.WriteAllText("input.txt", "A,B,C\n10,20,30\n40,50,60");

                // Ladeoptionen mit benutzerdefiniertem Light‑Cells‑Handler erstellen
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Arbeitsmappe mit benutzerdefiniertem Handler laden
                Workbook workbook = new Workbook("input.txt", loadOptions);

                // Verarbeitete Ergebnisse speichern
                workbook.Save("output.xlsx");
                Console.WriteLine("ProcessCell executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ProcessCell: {ex.Message}");
            }
        }

        private class CustomLightCellsDataHandler : LightCellsDataHandler
        {
            public bool StartSheet(Worksheet sheet)
            {
                return true; // Process all sheets
            }

            public bool StartRow(int rowIndex)
            {
                return true; // Process all rows
            }

            public bool StartCell(int columnIndex)
            {
                return true; // Process all cells
            }

            public bool ProcessCell(Cell cell)
            {
                // Numerische Werte verdoppeln und Zeichenketten markieren
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                else if (cell.Type == CellValueType.IsString)
                {
                    cell.PutValue($"TEXT: {cell.StringValue}");
                }
                return true;
            }

            public bool ProcessRow(Row row)
            {
                return true; // Continue processing
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


