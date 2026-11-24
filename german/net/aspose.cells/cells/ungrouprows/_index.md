---
title: "Cells.UngroupRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gruppierung von Zeilen aufheben"
type: docs
url: /de/net/aspose.cells/cells/ungrouprows/
---
## UngroupRows(int, int, bool) {#ungrouprows_1}

Löst die Gruppierung von Zeilen auf.

```csharp
public void UngroupRows(int firstIndex, int lastIndex, bool isAll)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | Int32 | Der Index der ersten Zeile, die entgruppiert werden soll. |
| lastIndex | Int32 | Der Index der letzten Zeile, die entgruppiert werden soll. |
| isAll | Boolean | True entfernt alle Gruppierungsinformationen. Andernfalls wird die äußere Gruppierungsinformation entfernt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUngroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Verschachtelte Zeilengruppierungen zum Demonstrationszweck erstellen
            worksheet.Cells.GroupRows(5, 7);  // First level grouping
            worksheet.Cells.GroupRows(5, 7);  // Second level grouping

            try
            {
                // Alle Ebenen der Zeilen 5-7 entgruppieren
                worksheet.Cells.UngroupRows(5, 7, true);

                Console.WriteLine("Rows 5-7 successfully ungrouped with all levels removed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UngroupRows: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("UngroupRowsWithBooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## UngroupRows(int, int) {#ungrouprows}

Löst die Gruppierung von Zeilen auf.

```csharp
public void UngroupRows(int firstIndex, int lastIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | Int32 | Der Index der ersten Zeile, die entgruppiert werden soll. |
| lastIndex | Int32 | Der Index der letzten Zeile, die entgruppiert werden soll. |

### Hinweise

Entfernt nur die äußere Gruppierungsinformation.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Einige Daten befüllen
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue($"Row {i}");
            }

            // Zeilen 1 bis 3 gruppieren (0-basierter Index)
            cells.GroupRows(1, 3, true);

            Console.WriteLine("Rows grouped from index 1 to 3");

            // Gruppierung der gleichen Zeilen aufheben
            cells.UngroupRows(1, 3);

            Console.WriteLine("Rows ungrouped from index 1 to 3");

            // Speichere die Arbeitsmappe
            workbook.Save("UngroupRowsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


