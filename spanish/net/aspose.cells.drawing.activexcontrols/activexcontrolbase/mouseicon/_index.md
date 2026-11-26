---
title: "ActiveXControlBase.MouseIcon"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Obtiene y establece un ícono personalizado para mostrar como puntero del mouse del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/
---
## ActiveXControlBase.MouseIcon property

Obtiene y establece un ícono personalizado para mostrar como puntero del mouse para el control.

```csharp
public byte[] MouseIcon { get; set; }
```

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System.IO;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyMouseIconDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 0, 1, 0, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            imageControl.MouseIcon = File.ReadAllBytes("mouse.ico");
            imageControl.MousePointer = ControlMousePointerType.Custom;

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


