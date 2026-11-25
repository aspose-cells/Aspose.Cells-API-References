---
title: "TextBoxActiveXControl.IsAutoWordSelected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Specifica l'unità di base usata per estendere una selezione. True indica che l'unità di base è un singolo carattere. false indica che l'unità di base è una parola intera"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautowordselected/
---
## TextBoxActiveXControl.IsAutoWordSelected property

Specifica l'unità di base utilizzata per estendere una selezione. True specifica che l'unità di base è un singolo carattere. false specifica che l'unità di base è una parola intera.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsAutoWordSelectedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 0, 0, 1, 1, 200, 30);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)textBoxShape.ActiveXControl;

            Console.WriteLine("Initial IsAutoWordSelected: " + textBoxControl.IsAutoWordSelected);

            if (!textBoxControl.IsAutoWordSelected)
            {
                textBoxControl.IsAutoWordSelected = true;
            }

            Console.WriteLine("Final IsAutoWordSelected: " + textBoxControl.IsAutoWordSelected);
        }
    }
}
```

### Vedi anche

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


