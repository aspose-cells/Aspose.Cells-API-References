---
title: "Cells.SetColumnWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Legt die Breite der angegebenen Spalte in der Normalansicht fest"
type: docs
url: /de/net/aspose.cells/cells/setcolumnwidth/
---
## Cells.SetColumnWidth method

Setzt die Breite der angegebenen Spalte in der Normalansicht.

```csharp
public void SetColumnWidth(int column, double width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex. |
| Breite | Double | Breite der Spalte in Zeichen. Die Spaltenbreite muss zwischen 0 und 255 liegen. |

### Hinweise

Bei Tabellenkalkulationen wird die Spaltenbreite als die Anzahl der Zeichen der maximalen Ziffernbreite der Zahlen 0~9 gemessen, wie sie in der Schriftart des normalen Stils dargestellt werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetColumnWidth(0, 25.5);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


