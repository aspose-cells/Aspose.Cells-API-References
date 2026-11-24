---
title: "Cells.SetRowHeightInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Setzt die Zeilenhöhe in der Einheit Zoll"
type: docs
url: /de/net/aspose.cells/cells/setrowheightinch/
---
## Cells.SetRowHeightInch method

Setzt die Zeilenhöhe in Zoll.

```csharp
public void SetRowHeightInch(int row, double inches)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |
| Zoll | Double | Anzahl der Zoll. Sie sollte zwischen 0 und 409,5/72 liegen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Standardstil festlegen
            Style style = workbook.DefaultStyle;
            style.Font.Name = "Tahoma";
            style.Font.Size = 16;
            style.Font.IsBold = true;
            workbook.DefaultStyle = style;

            // Zeilenhöhen in Zoll festlegen
            for (int i = 0; i < 10; i++)
            {
                cells.SetRowHeightInch(i, 0.5 + (i * 0.2)); // Demonstrates SetRowHeightInch(Int32, Double)
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RowHeightsInInches.xlsx");
            
            Console.WriteLine("Row heights set successfully in inches.");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


