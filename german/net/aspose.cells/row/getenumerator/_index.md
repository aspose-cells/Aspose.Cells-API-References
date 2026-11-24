---
title: "Row.GetEnumerator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Methode. Gibt den Zellen-Enumerator zurück"
type: docs
url: /de/net/aspose.cells/row/getenumerator/
---
## GetEnumerator() {#getenumerator}

Gibt den Zellen-Enumerator zurück

```csharp
public IEnumerator GetEnumerator()
```

### Rückgabewert

Der Zellen-Enumerator, der alle vorhandenen Zellen in dieser Zeile durchläuft.

### Beispiele

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Einige Beispieldaten einfügen
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            // Enumerator für die erste Zeile (Kopfzeile) abrufen
            IEnumerator en = cells.Rows[0].GetEnumerator();
            while (en.MoveNext())
            {
                Cell cell = (Cell)en.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Gibt einen Enumerator zurück, der die Zellen dieser Zeile durchläuft.

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| umgekehrt | Boolean | ob Zellen in umgekehrter Reihenfolge enumeriert werden |
| synchronisieren | Boolean | ob der zurückgegebene Enumerator Änderungen an den Zellen in dieser Zeile prüfen und synchronisieren soll. |

### Rückgabewert

Der Zellen-Enumerator, der alle vorhandenen Zellen in dieser Zeile durchläuft.

### Hinweise

Wenn die Zeile während der Durchquerung mit dem Enumerator geändert wird (durch Vorgänge, die dazu führen können, dass ein neuer Cell erstellt oder ein vorhandener Cell entfernt wird), sollte ein synchronisierter Enumerator anstelle eines normalen Enumerators verwendet werden, damit die Durchquerung ab der Position fortgesetzt werden kann, die unmittelbar nach der zuletzt von MoveNext() durchlaufenen liegt. Allerdings besteht neben dem Vorteil, dass kein Element übersprungen oder mehrfach durchlaufen wird, ein Nachteil des synchronisierten Enumerators darin, dass die Leistung im Vergleich zu einem normalen Enumerator etwas reduziert ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Daten zu Zellen in der ersten Zeile hinzu
            Row row = worksheet.Cells.Rows[0];
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            try
            {
                // Rufen Sie GetEnumerator mit reversed=false und sync=true auf
                IEnumerator enumerator = row.GetEnumerator(false, true);
                
                Console.WriteLine("Cells in row 1:");
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }

                // Rufen Sie GetEnumerator mit reversed=true und sync=false auf, um die umgekehrte Iteration zu demonstrieren
                Console.WriteLine("\nCells in row 1 (reversed order):");
                enumerator = row.GetEnumerator(true, false);
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RowMethodGetEnumeratorWithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


