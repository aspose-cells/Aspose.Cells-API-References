---
title: "CellsHelper.CellNameToIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Gibt die Zeilen- und Spaltenindizes der Zelle basierend auf ihrem Namen zurück."
type: docs
url: /de/net/aspose.cells/cellshelper/cellnametoindex/
---
## CellsHelper.CellNameToIndex method

Ermittelt die Zeilen- und Spaltenindizes der Zelle anhand ihres Namens.

```csharp
public static void CellNameToIndex(string cellName, out int row, out int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Name der Zelle. |
| row | Int32& | Ausgabe-Zeilenindex |
| column | Int32& | Ausgabe-Spaltenindex |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodCellNameToIndexWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Initialisieren Sie Variablen zum Halten von Zeilen- und Spaltenindizes.
            int rowIndex = -1;
            int columnIndex = -1;
            string cellName = "C5";

            try
            {
                // Rufen Sie die Methode CellNameToIndex auf, um den Zellnamen in Zeilen- und Spaltenindizes zu konvertieren.
                CellsHelper.CellNameToIndex(cellName, out rowIndex, out columnIndex);

                // Ergebnisse anzeigen
                Console.WriteLine($"Cell name: {cellName}");
                Console.WriteLine($"Row index: {rowIndex}");
                Console.WriteLine($"Column index: {columnIndex}");

                // Erstellen Sie eine Arbeitsmappe und demonstrieren Sie die Verwendung der Indizes.
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Greifen Sie mit den erhaltenen Indizes auf die Zelle zu.
                Cell cell = worksheet.Cells[rowIndex, columnIndex];
                cell.PutValue("Test Value");

                // Speichere die Arbeitsmappe
                workbook.Save("CellNameToIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CellNameToIndex method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


