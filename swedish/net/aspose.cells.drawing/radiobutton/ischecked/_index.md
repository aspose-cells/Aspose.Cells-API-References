---
title: "RadioButton.IsChecked"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RadioButton‑egenskap. Anger om radioknappen är markerad eller inte"
type: docs
url: /sv/net/aspose.cells.drawing/radiobutton/ischecked/
---
## RadioButton.IsChecked property

Anger om radioknappen är markerad eller inte.

```csharp
public bool IsChecked { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en radioknapp i kalkylbladet
            Shape shape = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 100);
            RadioButton radioButton = (RadioButton)shape;
            
            // Ställ in radioknappens text
            radioButton.Text = "Option 1";
            
            // Initialt avmarkerad
            radioButton.IsChecked = false;
            Console.WriteLine("Radio button initially unchecked: " + radioButton.IsChecked);
            
            // Markera radioknappen
            radioButton.IsChecked = true;
            Console.WriteLine("Radio button after checking: " + radioButton.IsChecked);
            
            // Spara arbetsboken
            workbook.Save("RadioButtonExample.xlsx");
        }
    }
}
```

### Se även

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


