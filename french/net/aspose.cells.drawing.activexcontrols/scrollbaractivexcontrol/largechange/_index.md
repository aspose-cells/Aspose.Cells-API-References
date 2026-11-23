---
title: "ScrollBarActiveXControl.LargeChange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ScrollBarActiveXControl. Obtient et définit la quantité de variation de la propriété Position"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/largechange/
---
## ScrollBarActiveXControl.LargeChange property

Obtient et définit la quantité par laquelle la propriété Position change

```csharp
public int LargeChange { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyLargeChangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un contrôle ActiveX ScrollBar
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 30);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Définissez la propriété LargeChange
            scrollBar.LargeChange = 5;

            // Enregistrez le classeur
            workbook.Save("ScrollBarActiveXControlLargeChangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


