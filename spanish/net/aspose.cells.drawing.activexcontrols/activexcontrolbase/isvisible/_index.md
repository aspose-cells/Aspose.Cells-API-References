---
title: "ActiveXControlBase.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Indica si este control es visible"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/
---
## ActiveXControlBase.IsVisible property

Indica si este control es visible.

```csharp
public virtual bool IsVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 1, 100, 100);
            var listBox = shape.ActiveXControl;

            // Configurar propiedades básicas
            listBox.IsVisible = true; // Demonstrate IsVisible property
            Console.WriteLine("Initial visibility: " + listBox.IsVisible);
            listBox.IsVisible = false;
            Console.WriteLine("After setting to false: " + listBox.IsVisible);
            listBox.IsVisible = true;
            Console.WriteLine("After setting to true: " + listBox.IsVisible);

            // Guarda el libro de trabajo
            workbook.Save("ActiveXControlVisibilityDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


