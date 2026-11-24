---
title: "Row.SetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Methode. Setzt den Stil dieser Zeile"
type: docs
url: /de/net/aspose.cells/row/setstyle/
---
## Row.SetStyle method

Setzt den Stil dieser Zeile.

```csharp
public void SetStyle(Style style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Der Stil, der als Standardstil für Zellen in dieser Zeile verwendet wird. |

### Hinweise

Diese Methode setzt den angegebenen Stil nur als Standardstil für diese Zeile, ohne die Stileinstellungen der bereits vorhandenen Zellen in dieser Zeile zu ändern. Um die Stileinstellungen der vorhandenen Zellen gleichzeitig auf den angegebenen Stil zu aktualisieren, verwenden Sie bitte [`ApplyStyle`](../applystyle/)

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle und konfiguriere einen Stil
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Blue;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.DiagonalStripe;

            // Hole die erste Zeile und wende den Stil an
            Row row = worksheet.Cells.Rows[0];
            row.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("RowStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


