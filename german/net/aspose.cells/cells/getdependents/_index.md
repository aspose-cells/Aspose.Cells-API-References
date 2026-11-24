---
title: "Cells.GetDependents"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Alle Zellen abrufen, die sich auf die angegebene Zelle beziehen"
type: docs
url: /de/net/aspose.cells/cells/getdependents/
---
## Cells.GetDependents method

Alle Zellen erhalten, die sich auf die angegebene Zelle beziehen.

```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isAll | Boolean | Gibt an, ob andere Arbeitsblätter überprüft werden |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetDependentsWithBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispielhafte Formeln und Werte einrichten
            cells["A1"].PutValue(10);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=A1+B1";
            cells["D1"].Formula = "=B1*3";
            cells["F4"].Formula = "=A1*5";

            // Formeln berechnen
            workbook.CalculateFormula();

            // Direkte Abhängige der Zelle A1 (Zeile 0, Spalte 0) abrufen
            Cell[] directDependents = cells.GetDependents(false, 0, 0);
            Console.WriteLine("Direct dependents of A1:");
            foreach (Cell cell in directDependents)
            {
                Console.WriteLine(cell.Name);
            }

            // Alle Abhängigkeiten (einschließlich indirekter) der Zelle A1 (Zeile 0, Spalte 0) abrufen
            Cell[] allDependents = cells.GetDependents(true, 0, 0);
            Console.WriteLine("\nAll dependents of A1:");
            foreach (Cell cell in allDependents)
            {
                Console.WriteLine(cell.Name);
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


