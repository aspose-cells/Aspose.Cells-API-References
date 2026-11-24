---
title: "Cells.ApplyColumnStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Wendet Formate für eine ganze Spalte an"
type: docs
url: /de/net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

Wendet Formate für eine ganze Spalte an.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Der Spaltenindex. |
| Stil | Stil | Das Stil‑Objekt, das angewendet wird. |
| Flag | StyleFlag | Flags, die die angewendeten Formatierungseigenschaften angeben. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyColumnStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Erstelle einen Stil mit Rahmen
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Erstelle ein Stil-Flag, um nur Rahmen anzuwenden
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;

            // Wende den Stil auf Spalte 1 (Index 0) an
            cells.ApplyColumnStyle(0, style, sflag);

            // Speichere die Arbeitsmappe
            workbook.Save("ApplyColumnStyleOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


