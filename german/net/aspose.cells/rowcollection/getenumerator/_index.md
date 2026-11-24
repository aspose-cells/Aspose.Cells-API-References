---
title: "RowCollection.GetEnumerator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RowCollection-Methode. Gibt einen Enumerator zurück, der die Zeilen in dieser Sammlung durchläuft"
type: docs
url: /de/net/aspose.cells/rowcollection/getenumerator/
---
## GetEnumerator() {#getenumerator}

Ermittelt einen Enumerator, der die Zeilen dieser Sammlung durchläuft

```csharp
public IEnumerator GetEnumerator()
```

### Rückgabewert

Der Zeilenenumerator, der alle vorhandenen Zeilen in dieser Sammlung durchläuft.

### Beispiele

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie Zeilenhöhen zur Demonstration
            worksheet.Cells.SetRowHeight(0, 15);
            worksheet.Cells.SetRowHeight(1, 20);
            worksheet.Cells.SetRowHeight(2, 25);

            IEnumerator enumerator = worksheet.Cells.Rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine($"Row index: {row.Index}, Height: {row.Height}");
            }
        }
    }
}
```

### Siehe auch

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Ermittelt einen Enumerator, der die Zeilen dieser Sammlung durchläuft

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| umgekehrt | Boolean | ob Zeilen in umgekehrter Reihenfolge enumeriert werden sollen |
| synchronisieren | Boolean | ob der zurückgegebene Enumerator die Änderungen der Zeilensammlung prüfen und mit ihr synchronisiert bleiben soll. |

### Rückgabewert

Der Zeilenenumerator, der alle vorhandenen Zeilen in dieser Sammlung durchläuft.

### Hinweise

Wenn die Zeilensammlung während der Traversierung mit dem Enumerator geändert wird (durch Vorgänge, die dazu führen können, dass ein neuer Row instanziiert oder ein vorhandener Row entfernt wird), sollte ein synchronisierter Enumerator anstelle eines normalen Enumerators verwendet werden, damit die Traversierung von der Position unmittelbar nach der zuletzt von MoveNext() durchlaufenen Position fortgesetzt werden kann. Allerdings besteht neben dem Vorteil, dass kein Element übersprungen oder mehrfach durchlaufen wird, der Nachteil des synchronisierten Enumerators darin, dass die Leistung im Vergleich zum normalen Enumerator etwas beeinträchtigt wird.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispielsdaten zu den Zeilen hinzu
            for (int i = 0; i < 5; i++)
            {
                Row row = worksheet.Cells.Rows[i];
                row[0].PutValue($"Row {i + 1}");
            }
            
            try
            {
                // Rufen Sie die RowCollection ab
                RowCollection rows = worksheet.Cells.Rows;
                
                // Rufen Sie GetEnumerator mit den Parametern (reversed: true, sync: false) auf
                IEnumerator enumerator = rows.GetEnumerator(true, false);
                
                Console.WriteLine("Iterating rows in reverse order:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
                
                // Rufen Sie GetEnumerator mit den Parametern (reversed: false, sync: true) auf
                enumerator = rows.GetEnumerator(false, true);
                
                Console.WriteLine("\nIterating rows in normal order (synchronized):");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("RowCollectionGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


