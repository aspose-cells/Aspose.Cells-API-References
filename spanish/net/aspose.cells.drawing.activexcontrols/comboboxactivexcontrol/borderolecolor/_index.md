---
title: "ComboBoxActiveXControl.BorderOleColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Obtiene y establece el color OLE del fondo"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderolecolor/
---
## ComboBoxActiveXControl.BorderOleColor property

Obtiene y establece el color ole del fondo.

```csharp
public int BorderOleColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Obtener la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                1, 1, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Configurar propiedades básicas
            comboBox.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // Demostrar la propiedad BorderOleColor
            comboBox.BorderOleColor = ColorTranslator.ToOle(Color.Red); // Set border color to red
            
            // Establecer texto de ejemplo
            comboBox.Value = "Border Color Demo";

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxBorderColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


