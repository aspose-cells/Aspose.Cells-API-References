---
title: "DataSorter.Sort"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter-Methode. Sortiert die Daten des Bereichs"
type: docs
url: /de/net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Sortiert die Daten des Bereichs.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zellen | Zellen | Die Zellen enthalten den Datenbereich. |
| startRow | Int32 | Die Startzeile des Bereichs. |
| startColumn | Int32 | Die Startspalte des Bereichs. |
| endRow | Int32 | Die Endzeile des Bereichs. |
| endColumn | Int32 | Die Endspalte des Bereichs. |

### Rückgabewert

die ursprünglichen Indizes (absolute Position, zum Beispiel ist Spalte A 0, B ist 1, ...) der sortierten Zeilen/Spalten. Wenn keine Zeilen/Spalten durch diesen Sortiervorgang verschoben werden müssen, wird null zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Beispieldaten befüllen
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue(6 - i);
            }
            
            // Eine Zeile ausblenden, um das Sortieren mit ausgeblendeten Zeilen zu demonstrieren
            cells.Rows[1].IsHidden = true;
            
            // Sorter erstellen und konfigurieren
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Sort-Methode mit Cells und Int32-Parametern demonstrieren
            sorter.Sort(cells, 0, 0, 5, 0);
            
            // Ergebnisse in die Konsole ausgeben
            for (int i = 0; i < 6; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {cells[i, 0].IntValue}");
            }
            Console.WriteLine($"Is row 2 hidden? {cells.Rows[1].IsHidden}");
        }
    }
}
```

### Siehe auch

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Sortiere die Daten des Bereichs.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zellen | Zellen | Die Zellen enthalten den Datenbereich. |
| Bereich | CellArea | Der zum Sortieren benötigte Bereich |

### Rückgabewert

die ursprünglichen Indizes (absolute Position, zum Beispiel ist Spalte A 0, B ist 1, ...) der sortierten Zeilen/Spalten. Wenn keine Zeilen/Spalten durch diesen Sortiervorgang verschoben werden müssen, wird null zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsCellAreaDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(1995);
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["A3"].PutValue(1996);
            worksheet.Cells["B3"].PutValue(15000);
            worksheet.Cells["A4"].PutValue(1997);
            worksheet.Cells["B4"].PutValue(12000);
            worksheet.Cells["A5"].PutValue(1998);
            worksheet.Cells["B5"].PutValue(18000);

            // Daten-Sortierer erstellen
            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.HasHeaders = true;
            dataSorter.Key1 = 0; // Sort by first column (Year)
            dataSorter.Order1 = SortOrder.Descending;

            // Sortierbereich definieren
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 1;

            // Sortierung durchführen
            dataSorter.Sort(worksheet.Cells, area);

            // Speichere die Arbeitsmappe
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Sortiere die Daten im Bereich.

```csharp
public int[] Sort()
```

### Rückgabewert

die ursprünglichen Indizes (absolute Position, zum Beispiel ist Spalte A 0, B ist 1, ...) der sortierten Zeilen/Spalten. Wenn keine Zeilen/Spalten durch diesen Sortiervorgang verschoben werden müssen, wird null zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Sortieren hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Ein Tabellen-/Listenobjekt erstellen
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Daten nach der ersten Spalte sortieren
            table.AutoFilter.Sorter.Sort();

            // Speichere die Arbeitsmappe
            workbook.Save("SortedData.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


