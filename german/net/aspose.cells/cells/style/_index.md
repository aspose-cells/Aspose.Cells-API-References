---
title: "Cells.Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Liest und setzt den Standardstil des Arbeitsblatts"
type: docs
url: /de/net/aspose.cells/cells/style/
---
## Cells.Style property

Liest und setzt den Standardstil des Arbeitsblatts.

```csharp
public Style Style { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setzen Sie einen Wert in Zelle A1
            Cell cell = cells["A1"];
            cell.PutValue(43368); // This represents the date 2018-09-25

            // Rufen Sie den Standardstil ab und ändern Sie dessen Format
            Style style = cells.Style;
            style.CultureCustom = "yyyymmdd!y";
            
            // Wende den geänderten Stil auf die Zelle an
            cell.SetStyle(style);

            // Den formatierten Zeichenkettenwert anzeigen
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


