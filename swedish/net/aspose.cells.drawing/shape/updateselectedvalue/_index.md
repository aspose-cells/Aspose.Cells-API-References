---
title: "Shape.UpdateSelectedValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-metod. Uppdatera det valda värdet med värdet från den länkade cellen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape.UpdateSelectedValue method

Uppdatera det valda värdet med värdet från den länkade cellen.

```csharp
public void UpdateSelectedValue()
```

### Exempel

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
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Skapa en ListBox-form
            Shape listBoxShape = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);
            
            // Ange inmatningsintervall och länkad cell
            listBoxShape.SetInputRange("$A$1:$A$6", false, false);
            listBoxShape.SetLinkedCell("$A$12", false, true);

            // Hämta ListBox-objektet
            ListBox listBox = (ListBox)listBoxShape;

            // Ange startvärde i den länkade cellen och uppdatera urvalet
            worksheet.Cells["A12"].Value = 3;
            listBoxShape.UpdateSelectedValue();

            // Verifiera urvalet
            if (listBox.IsSelected(2))
            {
                Console.WriteLine("Option 3 is selected");
            }

            // Ändra värde och uppdatera urvalet igen
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

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


