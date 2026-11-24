---
title: "LightCellsDataHandler.StartCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LightCellsDataHandler-Methode. Bereitet die Verarbeitung einer Zelle vor"
type: docs
url: /de/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

Bereitet die Verarbeitung einer Zelle vor.

```csharp
public bool StartCell(int columnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Spaltenindex der zu verarbeitenden Zelle |

### Rückgabewert

ob diese Zelle verarbeitet werden muss. false, um die Zelle zu ignorieren und die nächste zu prüfen, bis das Ende der Zellen‑Daten der aktuellen Zeile erreicht ist

### Hinweise

Sie wird aufgerufen, wenn eine vorhandene Zelle in der aktuellen Zeile erreicht wird. Die aktuelle Zeile ist die Zeile des letzten Aufrufs von [`ProcessRow`](../processrow/).

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodStartCellWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine temporäre Eingabedatei
                File.WriteAllText("input.csv", "Column1,Column2,Column3\n1,2,3\n4,5,6");

                // Ladeoptionen mit benutzerdefiniertem Light‑Cells‑Handler erstellen
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Arbeitsmappe mit benutzerdefiniertem Handler laden
                Workbook workbook = new Workbook("input.csv", loadOptions);

                // Speichere die verarbeitete Arbeitsmappe
                workbook.Save("output.xlsx");
                Console.WriteLine("StartCell method executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartCell method: {ex.Message}");
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
                // Verarbeite nur Zellen im Spaltenindex 1 (zweite Spalte)
                return columnIndex == 1;
            }

            public bool ProcessCell(Cell cell)
            {
                // Verdopple den Wert der Zellen in der zweiten Spalte
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
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

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


