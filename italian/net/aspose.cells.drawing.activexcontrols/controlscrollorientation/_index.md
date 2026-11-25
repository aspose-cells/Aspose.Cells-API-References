---
title: "Enum ControlScrollOrientation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.ActiveXControls.ControlScrollOrientation. Rappresenta il tipo di orientamento dello scorrimento"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlscrollorientation/
---
## ControlScrollOrientation enumeration

Rappresenta il tipo di orientamento dello scorrimento

```csharp
public enum ControlScrollOrientation
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Auto | `3` | Il controllo viene visualizzato orizzontalmente quando la larghezza del controllo è maggiore della sua altezza. Il controllo viene visualizzato verticalmente altrimenti. |
| Vertical | `0` | Il controllo viene visualizzato verticalmente. |
| Horizontal | `1` | Il controllo viene visualizzato orizzontalmente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollOrientationDemo
    {
        public static void ControlScrollOrientationExample()
        {
            // Inizializza una nuova cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi un ScrollBarActiveXControl al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 50);
            ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà per il ScrollBarActiveXControl
            activeXControl.LargeChange = 5;
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            // Dimostra come impostare l'orientamento usando l'enum ControlScrollOrientation
            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Salva la cartella di lavoro
            workbook.Save("ControlScrollOrientationExample.xlsx");
            workbook.Save("ControlScrollOrientationExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


