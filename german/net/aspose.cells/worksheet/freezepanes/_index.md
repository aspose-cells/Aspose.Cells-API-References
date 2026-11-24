---
title: "Worksheet.FreezePanes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Friert die Bereiche an der angegebenen Zelle im Arbeitsblatt ein"
type: docs
url: /de/net/aspose.cells/worksheet/freezepanes/
---
## FreezePanes(int, int, int, int) {#freezepanes}

Friert die Bildschirmelemente an der angegebenen Zelle im Arbeitsblatt ein.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |
| column | Int32 | Spaltenindex. |
| freezedRows | Int32 | Anzahl der sichtbaren Zeilen im oberen Bereich, nicht mehr als Zeilenindex. |
| freezedColumns | Int32 | Anzahl der sichtbaren Spalten im linken Bereich, nicht mehr als Spaltenindex. |

### Hinweise

Zeilenindex und Spaltenindex können nicht alle Null sein. Die Anzahl der Zeilen und die Anzahl der Spalten können ebenfalls nicht alle Null sein.

Die ersten beiden Parameter geben die eingefrorene Position an und die letzten beiden Parameter geben den im linken oberen Bereich eingefrorenen Bereich an.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fenster bei Zeile 3, Spalte 3 einfrieren, mit 3 eingefrorenen Zeilen und 3 eingefrorenen Spalten.
            worksheet.FreezePanes(3, 3, 3, 3);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## FreezePanes(string, int, int) {#freezepanes_1}

Friert die Bildschirmelemente an der angegebenen Zelle im Arbeitsblatt ein.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Zellname. |
| freezedRows | Int32 | Anzahl der sichtbaren Zeilen im oberen Bereich, nicht mehr als Zeilenindex. |
| freezedColumns | Int32 | Anzahl der sichtbaren Spalten im linken Bereich, nicht mehr als Spaltenindex. |

### Hinweise

Zeilenindex und Spaltenindex können nicht alle Null sein. Die Anzahl der Zeilen und die Anzahl der Spalten können ebenfalls nicht alle Null sein.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fenster bei "C3" einfrieren, mit 3 eingefrorenen Zeilen und 3 eingefrorenen Spalten.
            worksheet.FreezePanes("C3", 3, 3);

            // Speichere die Arbeitsmappe
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


