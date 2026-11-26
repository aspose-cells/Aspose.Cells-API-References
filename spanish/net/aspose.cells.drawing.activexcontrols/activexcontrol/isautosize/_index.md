---
title: "ActiveXControl.IsAutoSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ActiveXControl. Indica si el control cambiará de tamaño automáticamente para mostrar todo su contenido"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/
---
## ActiveXControl.IsAutoSize property

Indica si el control cambiará de tamaño automáticamente para mostrar todo su contenido.

```csharp
public virtual bool IsAutoSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Se corrigieron los parámetros de AddActiveXControl con la firma completa
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 0, 0, 100, 50);
            ActiveXControl control = shape.ActiveXControl;

            Console.WriteLine("Initial IsAutoSize: " + control.IsAutoSize);
            control.IsAutoSize = true;
            Console.WriteLine("Set IsAutoSize: " + control.IsAutoSize);

            string outputPath = "AutoSizeControlDemo.xlsm";
            workbook.Save(outputPath, SaveFormat.Xlsm);

            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ActiveXControl loadedControl = loadedShape.ActiveXControl;
            Console.WriteLine("Loaded IsAutoSize: " + loadedControl.IsAutoSize);
        }
    }
}
```

### Ver también

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


