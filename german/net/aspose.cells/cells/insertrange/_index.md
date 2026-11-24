---
title: "Cells.InsertRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption"
type: docs
url: /de/net/aspose.cells/cells/insertrange/
---
## InsertRange(CellArea, int, ShiftType, bool) {#insertrange_2}

Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType, bool updateReference)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | CellArea | Verschiebungsbereich. |
| shiftNumber | Int32 | Anzahl der einzufügenden Zeilen oder Spalten. |
| shiftType | ShiftType | Verschiebe‑Zellen‑Option. |
| updateReference | Boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Einige Beispieldaten einfügen
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);

            // Definiere den einzufügenden Bereich (Zeilen 2‑3, Spalte A)
            CellArea area = CellArea.CreateCellArea(1, 0, 2, 0);

            // Füge Bereich ein, verschiebe Zellen nach rechts und aktualisiere Verweise
            cells.InsertRange(area, 1, ShiftType.Right, true);

            // Überprüfe den Vorgang, indem du die Werte prüfst
            Console.WriteLine("A2 value after insert: " + cells["A2"].StringValue);
            Console.WriteLine("B2 value after insert: " + cells["B2"].StringValue);
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, ShiftType) {#insertrange}

Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption.

```csharp
public void InsertRange(CellArea area, ShiftType shiftType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | CellArea | Verschiebungsbereich. |
| shiftType | ShiftType | Verschiebe‑Zellen‑Option. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaShiftTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fülle einige Beispieldaten ein
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"R{row}C{col}");
                }
            }

            // Definiere den einzufügenden Zellbereich
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.EndRow = 4;
            area.StartColumn = 1;
            area.EndColumn = 3;

            // Füge Bereich ein und verschiebe Zellen nach unten
            cells.InsertRange(area, ShiftType.Down);

            // Speichere die Arbeitsmappe
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, int, ShiftType) {#insertrange_1}

Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | CellArea | Verschiebungsbereich. |
| shiftNumber | Int32 | Anzahl der einzufügenden Zeilen oder Spalten. |
| shiftType | ShiftType | Verschiebe‑Zellen‑Option. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Original Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["C1"].PutValue(200);
            
            // Definiere den einzufügenden Zellbereich (einzelne Zelle B1)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 1;
            area.EndColumn = 1;
            
            // Füge Bereich ein, verschiebe Zellen nach rechts
            worksheet.Cells.InsertRange(area, 1, ShiftType.Right);
            
            // Speichere die Arbeitsmappe
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


