---
title: "Cells.InsertColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Fügt dem Arbeitsblatt eine neue Spalte ein"
type: docs
url: /de/net/aspose.cells/cells/insertcolumn/
---
## InsertColumn(int, bool) {#insertcolumn_1}

Fügt eine neue Spalte in das Arbeitsblatt ein.

```csharp
public void InsertColumn(int columnIndex, bool updateReference)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Spaltenindex. |
| updateReference | Boolean | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fülle einige Beispieldaten in Spalte 0
            Cells cells = sheet.Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue($"Original {i}");
            }

            // Füge an Index 1 eine neue Spalte ein und verschiebe die Spalten nach rechts
            cells.InsertColumn(1, true);

            // Kopiere Daten von Spalte 0 in die neue Spalte 1
            cells.CopyColumn(cells, 0, 1);

            // Speichere die Arbeitsmappe
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumn(int) {#insertcolumn}

Fügt eine neue Spalte in das Arbeitsblatt ein.

```csharp
public void InsertColumn(int columnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Spaltenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet sheet = workbook.Worksheets[0];
            
            // Hole die Zellen-Sammlung
            Cells cells = sheet.Cells;
            
            // Füge Daten in Zellen zum Demonstrieren ein
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // Füge an Index 1 eine neue Spalte ein (wird die neue Spalte B)
            cells.InsertColumn(1);
            
            // Überprüfe, indem Daten in die neue Spalte eingefügt werden
            cells["B1"].PutValue("New Column");
            
            // Speichere die Arbeitsmappe
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


