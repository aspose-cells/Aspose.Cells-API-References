---
title: "Shape.ActiveXControl"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient le contrôle ActiveX"
type: docs
url: /fr/net/aspose.cells.drawing/shape/activexcontrol/
---
## Shape.ActiveXControl property

Obtient le contrôle ActiveX.

```csharp
public ActiveXControl ActiveXControl { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ShapePropertyActiveXControlDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 0, 0, 0, 0, 100, 30);

            if (shape.ActiveXControl != null)
            {
                CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
                string fontName = checkBox.Font.Name;
                Console.WriteLine($"CheckBox Font: {fontName}");
            }
        }
    }
}
```

### Voir aussi

* class [ActiveXControl](../../../aspose.cells.drawing.activexcontrols/activexcontrol/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


