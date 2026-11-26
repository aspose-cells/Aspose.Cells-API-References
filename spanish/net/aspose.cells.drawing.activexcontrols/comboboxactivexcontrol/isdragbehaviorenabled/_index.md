---
title: "ComboBoxActiveXControl.IsDragBehaviorEnabled"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Indica si el arrastre y la suelta están habilitados para el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isdragbehaviorenabled/
---
## ComboBoxActiveXControl.IsDragBehaviorEnabled property

Indica si arrastrar y soltar está habilitado para el control.

```csharp
public bool IsDragBehaviorEnabled { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsDragBehaviorEnabledDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer algunas propiedades básicas
            comboBox.ListRows = 8;
            comboBox.ColumnCount = 1;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = -1;

            // Demostrar la propiedad IsDragBehaviorEnabled
            Console.WriteLine("Initial IsDragBehaviorEnabled: " + comboBox.IsDragBehaviorEnabled);
            
            // Desactivar el comportamiento de arrastre
            comboBox.IsDragBehaviorEnabled = false;
            Console.WriteLine("After setting to false: " + comboBox.IsDragBehaviorEnabled);
            
            // Activar el comportamiento de arrastre
            comboBox.IsDragBehaviorEnabled = true;
            Console.WriteLine("After setting to true: " + comboBox.IsDragBehaviorEnabled);

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


