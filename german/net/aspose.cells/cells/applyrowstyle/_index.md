---
title: "Cells.ApplyRowStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Wendet Formate für eine ganze Zeile an"
type: docs
url: /de/net/aspose.cells/cells/applyrowstyle/
---
## Cells.ApplyRowStyle method

Wendet Formate für eine ganze Zeile an.

```csharp
public void ApplyRowStyle(int row, Style style, StyleFlag flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| Stil | Stil | Das Stil‑Objekt, das angewendet wird. |
| Flag | StyleFlag | Flags, die die angewendeten Formatierungseigenschaften angeben. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyRowStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstelle einen Stil mit Rahmen
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Erstellen Sie ein Stil-Flag für Rahmen
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Stil auf die erste Zeile anwenden
            cells.ApplyRowStyle(0, style, styleFlag);

            // Speichere die Arbeitsmappe
            workbook.Save("ApplyRowStyleDemo.xlsx");
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


