---
title: "EquationNodeParagraph.Justification"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "EquationNodeParagraph‑Eigenschaft. Sie gibt die Ausrichtung des mathematischen Absatzes an, einer Reihe benachbarter Gleichungen innerhalb desselben Absatzes. Ein mathematischer Absatz kann linksbündig, rechtsbündig, zentriert oder als Gruppe zentriert sein. Standardmäßig ist der mathematische Absatz als Gruppe zentriert. Das bedeutet, dass die Gleichungen zueinander ausgerichtet werden können, aber die gesamte Gruppe von Gleichungen als Ganzes zentriert ist."
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnodeparagraph/justification/
---
## EquationNodeParagraph.Justification property

Dies gibt die Ausrichtung des mathematischen Absatzes an (eine Reihe benachbarter Gleichungen innerhalb desselben Absatzes). Ein mathematischer Absatz kann linksbündig, rechtsbündig, zentriert oder als Gruppe zentriert sein. Standardmäßig ist der mathematische Absatz als Gruppe zentriert. Das bedeutet, dass die Gleichungen zueinander ausgerichtet werden können, aber die gesamte Gruppe von Gleichungen als Ganzes zentriert ist.

```csharp
public EquationHorizontalJustificationType Justification { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphPropertyJustificationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form erstellen, um die Gleichung zu enthalten
            var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

            // Den Gleichungsabsatz abrufen
            var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

            // Aktuellen Ausrichtungswert anzeigen
            Console.WriteLine("Current Justification value: " + equationParagraph.Justification);

            // Verschiedene Ausrichtungswerte festlegen und die Auswirkungen beobachten
            equationParagraph.Justification = EquationHorizontalJustificationType.Left;
            Console.WriteLine("Set to Left justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Center;
            Console.WriteLine("Set to Center justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.CenterGroup;
            Console.WriteLine("Set to CenterGroup justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Right;
            Console.WriteLine("Set to Right justification");

            // Speichere die Arbeitsmappe
            workbook.Save("EquationJustificationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [EquationHorizontalJustificationType](../../equationhorizontaljustificationtype/)
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


