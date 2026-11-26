---
title: "ActiveXControlBase.LinkedCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Obtiene y establece la celda vinculada"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/
---
## ActiveXControlBase.LinkedCell property

Obtiene y establece la celda vinculada.

```csharp
public string LinkedCell { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar un SpinButtonActiveXControl a la primera hoja de cálculo
            Aspose.Cells.Drawing.Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 
                10, 10, 100, 30, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;

            // Configurar las propiedades del botón giratorio
            spinButton.Min = 0;
            spinButton.Max = 100;
            spinButton.Position = 50;
            spinButton.SmallChange = 1;

            // Vincular el control a la celda A1
            spinButton.LinkedCell = "A1";

            // Establecer el valor de la celda A1 para que coincida con la posición inicial
            workbook.Worksheets[0].Cells["A1"].PutValue(spinButton.Position);

            // Guarda el libro de trabajo
            workbook.Save("LinkedCellDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


