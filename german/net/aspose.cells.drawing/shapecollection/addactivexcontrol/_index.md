---
title: "ShapeCollection.AddActiveXControl"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Erstellt ein Activex-Steuerelement"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/addactivexcontrol/
---
## ShapeCollection.AddActiveXControl method

Erstellt ein Activex-Steuerelement.

```csharp
public Shape AddActiveXControl(ControlType type, int topRow, int top, int leftColumn, int left, 
    int width, int height)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ControlType | Der Typ des Steuerelements. |
| topRow | Int32 | Index der oberen linken Zeile. |
| oben | Int32 | Stellt den vertikalen Versatz der Shape von ihrer linken Zeile dar, in Pixeln. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| links | Int32 | Stellt den horizontalen Versatz der Shape von ihrer linken Spalte dar, in Pixeln. |
| Höhe | Int32 | Stellt die Höhe der Shape dar, in Pixeln. |
| Breite | Int32 | Stellt die Breite der Shape dar, in Pixeln. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddActiveXControlWithControlTypeInt32Int32Int32Int3Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape activeXControl = shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 
                1,  // upperLeftRow
                0,  // top
                1,  // upperLeftColumn
                0,  // left
                100,  // width
                50   // height
            );

            workbook.Save("AddActiveXControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* enum [ControlType](../../../aspose.cells.drawing.activexcontrols/controltype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


