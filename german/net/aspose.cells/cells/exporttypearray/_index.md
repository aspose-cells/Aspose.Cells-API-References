---
title: "Cells.ExportTypeArray"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Exportiert den Zellenwerttyp in der Cells-Sammlung in ein zweidimensionales Array-Objekt"
type: docs
url: /de/net/aspose.cells/cells/exporttypearray/
---
## Cells.ExportTypeArray method

Exportiert den Zellenwerttyp in der [`Cells`](../)-Sammlung in ein zweidimensionales Array-Objekt.

```csharp
public CellValueType[] ExportTypeArray(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Die Zeilennummer der ersten zu exportierenden Zelle. |
| firstColumn | Int32 | Die Spaltennummer der ersten zu exportierenden Zelle. |
| totalRows | Int32 | Anzahl der zu exportierenden Zeilen. |
| totalColumns | Int32 | Anzahl der zu exportierenden Spalten. |

### Rückgabewert

Exportiertes Array-Objekt, das Zellenwerttypen darstellt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportTypeArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Werte in Cells setzen
            cells["A1"].PutValue(10);
            cells["B1"].PutValue("Hello");
            cells["A2"].PutValue(true);
            cells["B2"].PutValue(DateTime.Now);

            // Exportiere Zellentypen in ein 2D-Array
            CellValueType[,] typeArray = cells.ExportTypeArray(0, 0, 2, 2);

            // Ergebnisse anzeigen
            for (int i = 0; i < 2; i++)
            {
                for (int j = 0; j < 2; j++)
                {
                    Console.WriteLine($"Cell[{i},{j}] Type: {typeArray[i, j]}");
                }
            }

            // Ausnahmefall demonstrieren
            try
            {
                CellValueType[,] invalidArray = cells.ExportTypeArray(-1, 0, 2, 2);
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Exception caught as expected: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


