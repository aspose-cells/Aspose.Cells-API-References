---
title: "ActiveXControlBase.Width"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ActiveXControlBase. Obtient et définit la largeur du contrôle en points"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/width/
---
## ActiveXControlBase.Width property

Obtient et définit la largeur du contrôle en unité de points.

```csharp
public virtual double Width { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            ActiveXControlBase control = (ActiveXControlBase)shape.ActiveXControl;

            // Démontrer l’utilisation de la propriété Width
            Console.WriteLine("Original width: " + control.Width);
            control.Width = 150;
            Console.WriteLine("Modified width: " + control.Width);

            workbook.Save("ActiveXControlWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


