---
title: "Cells.GetColumnWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die Spaltenbreite zurück"
type: docs
url: /de/net/aspose.cells/cells/getcolumnwidth/
---
## GetColumnWidth(int, bool, CellsUnitType) {#getcolumnwidth_1}

Ermittelt die Spaltenbreite.

```csharp
public double GetColumnWidth(int column, bool isOriginal, CellsUnitType unitType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Der Spaltenindex. |
| isOriginal | Boolean | Gibt an, ob die ursprüngliche Breite abgerufen wird. |
| unitType | CellsUnitType |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setzt die Spaltenbreite für Spalte 1 (0-basierter Index)
            cells.SetColumnWidth(0, 20);

            // Ermittelt die Spaltenbreite in verschiedenen Einheiten und Modi
            double widthInPixels = cells.GetColumnWidth(0, true, CellsUnitType.Pixel);
            double widthInPoints = cells.GetColumnWidth(0, true, CellsUnitType.Point);
            double defaultWidth = cells.GetColumnWidth(0, false, CellsUnitType.Pixel);

            Console.WriteLine("Column width in pixels: " + widthInPixels);
            Console.WriteLine("Column width in points: " + widthInPoints);
            Console.WriteLine("Default column width: " + defaultWidth);
        }
    }
}
```

### Siehe auch

* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidth(int) {#getcolumnwidth}

Ermittelt die Breite (in Zeichen) der angegebenen Spalte in der Normalansicht.

```csharp
public double GetColumnWidth(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex |

### Rückgabewert

Spaltenbreite. In einer Tabellenkalkulation wird die Spaltenbreite als die Anzahl der Zeichen der maximalen Ziffernbreite der Zahlen 0~9 gemessen, wie sie in der Schriftart des normalen Stils dargestellt werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setzt die Spaltenbreite für Spaltenindex 255
            cells.SetColumnWidth(255, 20.86);

            // Ermittelt und zeigt die Spaltenbreite an
            double columnWidth = cells.GetColumnWidth(255);
            Console.WriteLine("Column width at index 255: " + columnWidth);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


