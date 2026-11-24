---
title: "StyleFlag.DiagonalUpBorder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Einstellungen für diagonalen oberen Rand werden angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/diagonalupborder/
---
## StyleFlag.DiagonalUpBorder property

Die Einstellungen für den diagonalen Aufwärtsrahmen werden angewendet.

```csharp
public bool DiagonalUpBorder { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalUpBorderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf Zelle A1 zu und setze etwas Text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Erstellen Sie ein Style-Objekt und setzen Sie den diagonalen oberen Rand
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 0, 255);

            // Erstellen Sie ein Style-Flag und aktivieren Sie das diagonale obere Rand-Flag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalUpBorder = true;

            // Den Stil mit dem Flag auf die Zelle anwenden
            cell.SetStyle(style, styleFlag);

            // Erstellen Sie eine weitere Zelle, um den Effekt zu demonstrieren
            Cell cell2 = worksheet.Cells["B2"];
            cell2.PutValue("Diagonal Up Border Demo");

            // Erstellen Sie einen anderen Stil zum Vergleich
            Style style2 = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 255, 0);

            // Wenden Sie den zweiten Stil mit demselben Flag an
            cell2.SetStyle(style2, styleFlag);

            // Speichere die Arbeitsmappe
            workbook.Save("StyleFlagPropertyDiagonalUpBorderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


