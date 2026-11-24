---
title: "Cells.CreateRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Erstellt ein Range-Objekt aus einem Zellbereich"
type: docs
url: /de/net/aspose.cells/cells/createrange/
---
## CreateRange(string, string) {#createrange_3}

Erstellt ein [`Range`](../../range/) Objekt aus einem Zellbereich.

```csharp
public Range CreateRange(string upperLeftCell, string lowerRightCell)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| upperLeftCell | String | Name der oberen linken Zelle. |
| lowerRightCell | String | Name der unteren rechten Zelle. |

### Rückgabewert

Ein [`Range`](../../range/) Objekt

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Erstelle einen Bereich von A1 bis A2
            Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
            range.Name = "MyRange";
            
            // Werte im Bereich festlegen
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            
            // Verwende den Bereich in einer Formel
            cells["B1"].Formula = "=SUM(MyRange)";
            
            // Formel berechnen
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of MyRange (A1:A2) is: " + cells["B1"].IntValue);
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, int, int) {#createrange_1}

Erstellt ein [`Range`](../../range/) Objekt aus einem Zellbereich.

```csharp
public Range CreateRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Erste Zeile dieses Bereichs |
| firstColumn | Int32 | Erste Spalte dieses Bereichs |
| totalRows | Int32 | Anzahl der Zeilen |
| totalColumns | Int32 | Anzahl der Spalten |

### Rückgabewert

Ein [`Range`](../../range/) Objekt

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstelle Quellbereich (beginnend bei Zeile 2, Spalte 2 mit 3 Zeilen und 4 Spalten)
            Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);

            // Fülle den Quellbereich mit Beispieldaten
            for (int i = 0; i < rangeSrc.RowCount; i++)
            {
                for (int j = 0; j < rangeSrc.ColumnCount; j++)
                {
                    rangeSrc[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Erstelle Zielbereich (beginnend bei Zeile 8, Spalte 0 mit gleichen Abmessungen)
            Aspose.Cells.Range rangeDest = cells.CreateRange(8, 0, 3, 4);

            // Kopiere Werte von der Quelle zum Ziel
            rangeDest.CopyValue(rangeSrc);

            // Speichere die Arbeitsmappe
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(string) {#createrange_2}

Erstellt ein [`Range`](../../range/) Objekt aus einer Adresse des Bereichs.

```csharp
public Range CreateRange(string address)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| address | String | Die Adresse des Bereichs. |

### Rückgabewert

Ein [`Range`](../../range/) Objekt

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Bereich mittels Zeichenkettenadresse
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Fülle Daten im Bereich
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Erstelle einen weiteren Bereich in einem neuen Arbeitsblatt
            workbook.Worksheets.Add();
            Worksheet worksheet2 = workbook.Worksheets[1];
            Aspose.Cells.Range range2 = worksheet2.Cells.CreateRange("A1:C3");

            // Kopiere Daten zwischen Bereichen
            range2.Copy(range);

            // Speichere die Arbeitsmappe
            workbook.Save("CreateRangeWithStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, bool) {#createrange}

Erstellt ein [`Range`](../../range/) Objekt aus Zeilen von Zellen oder Spalten von Zellen.

```csharp
public Range CreateRange(int firstIndex, int number, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | Int32 | Erster Zeilenindex oder erster Spaltenindex, nullbasiert. |
| Zahl | Int32 | Gesamtzahl der Zeilen oder Spalten, einsbasiert. |
| isVertical | Boolean | True - Bereich aus Spalten von Zellen erstellt. False - Bereich aus Zeilen von Zellen erstellt. |

### Rückgabewert

Ein [`Range`](../../range/) Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstelle einen Bereich, beginnend bei Zelle A1 (0,0) mit 5 Zeilen und 3 Spalten
            Aspose.Cells.Range range = cells.CreateRange(0, 0, true);

            // Füllen Sie einige Daten in den Bereich ein
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Row {i}, Col {j}");
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


