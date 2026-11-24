---
title: "Cells.DeleteRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Löscht mehrere Zeilen"
type: docs
url: /de/net/aspose.cells/cells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Löscht mehrere Zeilen.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Der Index der ersten zu löschenden Zeile. |
| totalRows | Int32 | Anzahl der zu löschenden Zeilen. |

### Hinweise

Wenn der gelöschte Bereich den oberen Teil (nicht das Ganze) der Tabelle (ListObject) enthält, kann der Bereich nicht gelöscht werden und es wird nichts unternommen. Es funktioniert auf dieselbe Weise wie in MS Excel.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Einige Beispieldaten einfügen
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            Console.WriteLine("Before deleting rows:");
            PrintCellValues(cells, 0, 9, 0, 4);

            // Lösche 2 Zeilen beginnend ab Zeilenindex 2 (3. Zeile)
            cells.DeleteRows(2, 2);

            Console.WriteLine("\nAfter deleting rows 3-4:");
            PrintCellValues(cells, 0, 7, 0, 4);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }

        private static void PrintCellValues(Cells cells, int startRow, int endRow, int startCol, int endCol)
        {
            for (int i = startRow; i <= endRow; i++)
            {
                for (int j = startCol; j <= endCol; j++)
                {
                    Console.Write($"{cells[i, j].StringValue}\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_2}

Löscht mehrere Zeilen im Arbeitsblatt.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Index der ersten zu löschenden Zeile. |
| totalRows | Int32 | Anzahl der zu löschenden Zeilen. |
| updateReference | Boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten in Zellen importieren
            worksheet.Cells.ImportTwoDimensionArray(new object[2, 2] { { "A1", "B1" }, { "A2", "B2" } }, 0, 0);

            // Eine Tabelle erstellen
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 1, 1, false)];
            table.ShowHeaderRow = false;

            Console.WriteLine("Before DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");

            // Lösche Zeile bei Index 1 (zweite Zeile) mit aktualisierter Referenz
            worksheet.Cells.DeleteRows(1, 1, true);

            Console.WriteLine("\nAfter DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, DeleteOptions) {#deleterows_1}

Löscht mehrere Zeilen im Arbeitsblatt.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, DeleteOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Index der ersten zu löschenden Zeile. |
| totalRows | Int32 | Anzahl der zu löschenden Zeilen. |
| Optionen | DeleteOptions | Optionen für den Löschvorgang |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Beispieldaten und Formeln festlegen
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].Formula = "=SUM(A1:A3)";
            
            // Zeile 2 ohne Überwachung löschen (da FormulaChangeMonitor nicht verfügbar ist)
            cells.DeleteRows(1, 1, new DeleteOptions());
            
            Console.WriteLine("Deleted row 2. Formula in B1 should now be: " + cells["B1"].Formula);
        }
    }
}
```

### Siehe auch

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


