---
title: "TextBoxActiveXControl.ScrollBars"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxActiveXControl. Indica se il controllo ha barre di scorrimento verticali, orizzontali, entrambe o nessuna"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars/
---
## TextBoxActiveXControl.ScrollBars property

Indica se il controllo ha barre di scorrimento verticali, barre di scorrimento orizzontali, entrambe o nessuna.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una nuova raccolta di forme e aggiungi il controllo ActiveX
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
            
            // Imposta la proprietà ScrollBars su verticale
            textBox.ScrollBars = ControlScrollBarType.BarsVertical;
            
            // Salva la cartella di lavoro
            workbook.Save("TextBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


