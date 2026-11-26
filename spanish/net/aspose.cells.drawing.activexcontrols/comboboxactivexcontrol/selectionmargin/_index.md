---
title: "ComboBoxActiveXControl.SelectionMargin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Indica si el usuario puede seleccionar una línea de texto haciendo clic en la zona a la izquierda del texto"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/selectionmargin/
---
## ComboBoxActiveXControl.SelectionMargin property

Indica si el usuario puede seleccionar una línea de texto haciendo clic en la zona a la izquierda del texto.

```csharp
public bool SelectionMargin { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertySelectionMarginDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Demostrar la propiedad SelectionMargin
            comboBox.SelectionMargin = false;
            Console.WriteLine("SelectionMargin set to: " + comboBox.SelectionMargin);

            // Alternar y demostrar de nuevo
            comboBox.SelectionMargin = true;
            Console.WriteLine("SelectionMargin now set to: " + comboBox.SelectionMargin);

            workbook.Save("ComboBoxSelectionMarginDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


