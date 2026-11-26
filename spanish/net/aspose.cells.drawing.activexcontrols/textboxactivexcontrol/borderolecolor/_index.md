---
title: "TextBoxActiveXControl.BorderOleColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Obtiene y establece el color ole del fondo"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderolecolor/
---
## TextBoxActiveXControl.BorderOleColor property

Obtiene y establece el color ole del fondo.

```csharp
public int BorderOleColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un control ActiveX TextBox y obtén su propiedad ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 1, 1, 100, 100, 100, 100);
            var textBox = (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad BorderOleColor (sistema de color predeterminado de Excel 12 o verde)
            textBox.BorderOleColor = unchecked((int)0x80000012);

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlBorderOleColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


