---
title: "Border.LineStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Border-Eigenschaft. Gibt den Zellenrahmentyp zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

Liest oder setzt den Zellenrandtyp.

```csharp
public CellBorderType LineStyle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyLineStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf eine Zelle zu und rufen Sie ihren Stil ab
            Cell cell = worksheet.Cells["B2"];
            Style style = cell.GetStyle();

            // Setzen Sie unterschiedliche Rahmenlinienstile
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;

            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("BorderLineStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


