---
title: "Cells.Merge"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Fügt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen"
type: docs
url: /de/net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Erste Zeile dieses Bereichs (nullbasiert) |
| firstColumn | Int32 | Erste Spalte dieses Bereichs (nullbasiert) |
| totalRows | Int32 | Anzahl der Zeilen (einsbasiert) |
| totalColumns | Int32 | Anzahl der Spalten (einsbasiert) |

### Hinweise

Referenziere die zusammengeführte Zelle über die Adresse der oberen linken Zelle im Bereich.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Werte in Zellen einfügen, um das Zusammenführen zu demonstrieren
            cells[0, 0].PutValue("Merged Area");
            cells[5, 5].PutValue("Not Merged");

            // Zellen zusammenführen, beginnend bei Zeile 0, Spalte 0, über 3 Zeilen und 2 Spalten
            cells.Merge(0, 0, 3, 2);

            // Speichere die Arbeitsmappe
            workbook.Save("MergeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Erste Zeile dieses Bereichs (nullbasiert) |
| firstColumn | Int32 | Erste Spalte dieses Bereichs (nullbasiert) |
| totalRows | Int32 | Anzahl der Zeilen (einsbasiert) |
| totalColumns | Int32 | Anzahl der Spalten (einsbasiert) |
| mergeConflict | Boolean | Zusammenführungs-Konflikt bei zusammengeführten Bereichen. |

### Hinweise

Referenziere die zusammengeführte Zelle über die Adresse der oberen linken Zelle im Bereich. Wenn mergeConflict true ist und der zusammengeführte Bereich mit anderen zusammengeführten Zellen kollidiert, werden die anderen zusammengeführten Zellen automatisch entfernt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zellen zusammenführen von Zeile 3, Spalte 4 (D3) bis Zeile 7, Spalte 5 (E7) – 5 Zeilen und 2 Spalten
            worksheet.Cells.Merge(3, 4, 5, 2, true);
            
            // Speichere die Arbeitsmappe
            workbook.Save("MergeDemoOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Erste Zeile dieses Bereichs (nullbasiert) |
| firstColumn | Int32 | Erste Spalte dieses Bereichs (nullbasiert) |
| totalRows | Int32 | Anzahl der Zeilen (einsbasiert) |
| totalColumns | Int32 | Anzahl der Spalten (einsbasiert) |
| checkConflict | Boolean | Gibt an, ob die zusammengeführten Zellen andere zusammengeführte Zellen überschneiden |
| mergeConflict | Boolean | Zusammenführungs-Konflikt bei zusammengeführten Bereichen. |

### Hinweise

Referenziere die zusammengeführte Zelle über die Adresse der oberen linken Zelle im Bereich. Wenn mergeConflict true ist und der zusammengeführte Bereich mit anderen zusammengeführten Zellen kollidiert, werden die anderen zusammengeführten Zellen automatisch entfernt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanBooDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Einige Daten in die zu zusammenzuführenden Zellen einfügen
            cells[0, 1].PutValue("Merged Cell");
            cells[1, 1].PutValue("This will be merged");

            // Zellen ohne Optionen zusammenführen (einfache Zusammenführung)
            cells.Merge(0, 1, 2, 2);
            Console.WriteLine("Cells merged without options");

            // Zuerst aufheben, um die nächste Zusammenführung zu demonstrieren
            cells.UnMerge(0, 1, 2, 2);

            // Zellen zusammenführen mit ignoreStyle=false und mergeConflict=true
            cells.Merge(0, 1, 2, 2, false, true);
            Console.WriteLine("Cells merged with ignoreStyle=false and mergeConflict=true");

            // Speichere die Arbeitsmappe
            workbook.Save("MergeCellsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


