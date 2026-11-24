---
title: "Shape.UpdateSelectedValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Aktualisieren Sie den ausgewählten Wert anhand des Werts der verknüpften Zelle"
type: docs
url: /de/net/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape.UpdateSelectedValue method

Aktualisiert den ausgewählten Wert anhand des Werts der verknüpften Zelle.

```csharp
public void UpdateSelectedValue()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten einfügen
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Erstellen Sie ein ListBox-Shape
            Shape listBoxShape = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);
            
            // Eingabebereich und verknüpfte Zelle festlegen
            listBoxShape.SetInputRange("$A$1:$A$6", false, false);
            listBoxShape.SetLinkedCell("$A$12", false, true);

            // Das ListBox-Objekt abrufen
            ListBox listBox = (ListBox)listBoxShape;

            // Anfangswert in verknüpfter Zelle festlegen und Auswahl aktualisieren
            worksheet.Cells["A12"].Value = 3;
            listBoxShape.UpdateSelectedValue();

            // Auswahl überprüfen
            if (listBox.IsSelected(2))
            {
                Console.WriteLine("Option 3 is selected");
            }

            // Wert ändern und Auswahl erneut aktualisieren
            worksheet.Cells["A12"].Value = 4;
            listBoxShape.UpdateSelectedValue();

            if (listBox.IsSelected(3))
            {
                Console.WriteLine("Option 4 is selected");
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


