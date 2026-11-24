---
title: "DataSorter.AddKey"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter-Methode. Fügt den Index der sortierten Spalte und die Sortierreihenfolge hinzu"
type: docs
url: /de/net/aspose.cells/datasorter/addkey/
---
## AddKey(int, SortOrder) {#addkey_1}

Fügt sortierten Spaltenindex und Sortierreihenfolge hinzu.

```csharp
public void AddKey(int key, SortOrder order)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | Int32 | Der sortierte Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...) |
| Reihenfolge | SortOrder | Die Sortierreihenfolge |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Sortierschlüssel für Spalte B (Index 1) mit aufsteigender Reihenfolge hinzufügen
            workbook.DataSorter.AddKey(1, SortOrder.Ascending);
            
            // Datenbereich sortieren (A1:B4)
            workbook.DataSorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Sortierte Werte ausgeben
            Console.WriteLine("Sorted by Age (Ascending):");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[$"A{i+1}"].StringValue}: {worksheet.Cells[$"B{i+1}"].IntValue}");
            }
        }
    }
}
```

### Siehe auch

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string) {#addkey_2}

Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu.

```csharp
public void AddKey(int key, SortOrder order, string customList)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | Int32 | Der sortierte Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...) |
| Reihenfolge | SortOrder | Die Sortierreihenfolge. |
| customList | String | Die benutzerdefinierte Sortierliste. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Sortieren
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("ddd");
            worksheet.Cells["A3"].PutValue("aaa");
            worksheet.Cells["A4"].PutValue("ccc");
            worksheet.Cells["A5"].PutValue("bbb");

            // Daten-Sortierer erstellen und benutzerdefinierten Sortierschlüssel hinzufügen
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
            sorter.HasHeaders = true;

            // Daten sortieren
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Ergebnis speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOnType, SortOrder, object) {#addkey}

Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu.

```csharp
public void AddKey(int key, SortOnType type, SortOrder order, object customList)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | Int32 | Der sortierte Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...) |
| Typ | SortOnType | Der Typ des sortierten Werts. |
| Reihenfolge | SortOrder | Die Sortierreihenfolge. |
| customList | Object | Die benutzerdefinierte Sortierliste. |

### Hinweise

Wenn der Typ SortOnType.CellColor oder SortOnType.FontColor ist, ist die customList eine Farbe.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Einen Daten-Sortierer erstellen
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;

            try
            {
                // AddKey mit Parametern aufrufen: (Int32, SortOnType, SortOrder, Object)
                sorter.AddKey(
                    1,                          // Column index (B column)
                    SortOnType.Value,           // Sort on values (fixed from Values to Value)
                    SortOrder.Ascending,        // Sort order
                    null                        // Custom list (null for default)
                );

                // Den zu sortierenden Bereich definieren
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 3;
                area.EndColumn = 1;

                // Daten sortieren
                sorter.Sort(worksheet.Cells, area);

                Console.WriteLine("Data sorted successfully using AddKey with parameters (Int32, SortOnType, SortOrder, Object)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddKey method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string[]) {#addkey_3}

Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu.

```csharp
public void AddKey(int key, SortOrder order, string[] customList)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schlüssel | Int32 | Der sortierte Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...) |
| Reihenfolge | SortOrder | Die Sortierreihenfolge. |
| customList | String[] | Die benutzerdefinierte Sortierliste. |

### Siehe auch

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


