---
title: "TextBoxActiveXControl.PasswordChar"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxActiveXControl-egenskap. Hämtar och anger ett tecken som ska visas i stället för de inmatade tecknen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/passwordchar/
---
## TextBoxActiveXControl.PasswordChar property

Hämtar och anger ett tecken som ska visas i stället för de inmatade tecknen.

```csharp
public char PasswordChar { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyPasswordCharDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox ActiveX Control och hämta dess form
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 0, 1, 1, 100, 50);
            
            // Hämta TextBoxActiveXControl från formen
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBoxControl = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Ställ in PasswordChar-egenskapen
            textBoxControl.PasswordChar = '*';

            // Ange lite text för att demonstrera lösenordsmaskering
            textBoxControl.Text = "password123";

            // Spara arbetsboken
            workbook.Save("TextBoxActiveXControlPasswordCharDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


