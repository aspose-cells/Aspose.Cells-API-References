---
title: "Cells.ExportArray"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Exportiert Daten aus der Cells-Sammlung in ein zweidimensionales Array-Objekt"
type: docs
url: /de/net/aspose.cells/cells/exportarray/
---
## Cells.ExportArray method

Exportiert Daten aus der [`Cells`](../)-Sammlung in ein zweidimensionales Array-Objekt.

```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Die Zeilennummer der ersten zu exportierenden Zelle. |
| firstColumn | Int32 | Die Spaltennummer der ersten zu exportierenden Zelle. |
| totalRows | Int32 | Anzahl der zu exportierenden Zeilen |
| totalColumns | Int32 | Anzahl der zu exportierenden Spalten |

### Rückgabewert

Exportiertes Zellwert-Array-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Einige Beispieldaten einfügen
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[1, 0].PutValue(10);
            cells[1, 1].PutValue(20);

            try
            {
                // Daten in ein Array exportieren
                object[,] dataArray = cells.ExportArray(0, 0, 2, 2);
                
                // Exportiertes Array anzeigen
                for (int i = 0; i < 2; i++)
                {
                    for (int j = 0; j < 2; j++)
                    {
                        Console.Write(dataArray[i, j] + "\t");
                    }
                    Console.WriteLine();
                }
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error exporting array: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


