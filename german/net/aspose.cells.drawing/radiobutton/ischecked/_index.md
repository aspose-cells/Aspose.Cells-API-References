---
title: "RadioButton.IsChecked"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RadioButton-Eigenschaft. Gibt an, ob das RadioButton aktiviert ist oder nicht"
type: docs
url: /de/net/aspose.cells.drawing/radiobutton/ischecked/
---
## RadioButton.IsChecked property

Gibt an, ob der RadioButton aktiviert ist oder nicht.

```csharp
public bool IsChecked { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonPropertyIsCheckedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge ein RadioButton zum Arbeitsblatt hinzu
            Shape shape = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 100);
            RadioButton radioButton = (RadioButton)shape;
            
            // Setze den Text des RadioButtons
            radioButton.Text = "Option 1";
            
            // Anfangs nicht aktiviert
            radioButton.IsChecked = false;
            Console.WriteLine("Radio button initially unchecked: " + radioButton.IsChecked);
            
            // Aktiviere das RadioButton
            radioButton.IsChecked = true;
            Console.WriteLine("Radio button after checking: " + radioButton.IsChecked);
            
            // Speichere die Arbeitsmappe
            workbook.Save("RadioButtonExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


