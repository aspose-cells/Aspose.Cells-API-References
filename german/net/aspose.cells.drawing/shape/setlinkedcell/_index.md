---
title: "Shape.SetLinkedCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Legt den Bereich fest, der mit dem Wert des Steuerelements verknüpft ist."
type: docs
url: /de/net/aspose.cells.drawing/shape/setlinkedcell/
---
## Shape.SetLinkedCell method

Legt den mit dem Wert der Steuerung verknüpften Bereich fest.

```csharp
public void SetLinkedCell(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Der Bereich, der mit dem Wert des Steuerelements verknüpft ist. |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLinkedCellWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Bildlaufleisten-Form hinzufügen
            Aspose.Cells.Drawing.Shape scrollBar = worksheet.Shapes.AddScrollBar(2, 0, 2, 0, 130, 30);

            // Verknüpfen Sie den Bildlaufleistenwert mit Zelle A12
            scrollBar.SetLinkedCell("$A$12", false, true);

            // Speichere die Arbeitsmappe
            workbook.Save("SetLinkedCellDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


