---
title: "TextBoxActiveXControl.IsAutoWordSelected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Especifica la unidad básica utilizada para ampliar una selección. True indica que la unidad básica es un solo carácter. false indica que la unidad básica es una palabra completa"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautowordselected/
---
## TextBoxActiveXControl.IsAutoWordSelected property

Especifica la unidad básica utilizada para ampliar una selección. True indica que la unidad básica es un solo carácter. false indica que la unidad básica es una palabra completa.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### Ejemplos

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

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


