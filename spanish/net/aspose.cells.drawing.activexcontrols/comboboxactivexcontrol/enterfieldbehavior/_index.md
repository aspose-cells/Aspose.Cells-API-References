---
title: "ComboBoxActiveXControl.EnterFieldBehavior"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Especifica el comportamiento de selección al entrar en el control. True indica que la selección permanece sin cambios desde la última vez que el control estuvo activo. False indica que todo el texto en el control se seleccionará al entrar en el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/enterfieldbehavior/
---
## ComboBoxActiveXControl.EnterFieldBehavior property

Especifica el comportamiento de selección al entrar al control. True indica que la selección permanece sin cambios desde la última vez que el control estuvo activo. False indica que todo el texto del control se seleccionará al entrar al control.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyEnterFieldBehaviorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar el primer control ActiveX ComboBox
            Shape shape1 = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 1, 0, 100, 50
            );
            ComboBoxActiveXControl combo1 = (ComboBoxActiveXControl)shape1.ActiveXControl;
            combo1.EnterFieldBehavior = false; // Default behavior (select all text on entry)
            combo1.Value = "Select Option";
            combo1.BorderStyle = ControlBorderType.Single;
            
            // Agregar el segundo control ActiveX ComboBox
            Shape shape2 = worksheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                1, 0, 2, 0, 100, 50
            );
            ComboBoxActiveXControl combo2 = (ComboBoxActiveXControl)shape2.ActiveXControl;
            combo2.EnterFieldBehavior = true; // Preserve previous selection
            combo2.Value = "Edit Value";
            combo2.BorderStyle = ControlBorderType.Single;
            
            // Guarda el libro de trabajo
            workbook.Save("ComboBoxActiveXControlDemo.xlsm", SaveFormat.Xlsm);
            
            // Verificar la configuración de la propiedad
            Console.WriteLine("Combo1 EnterFieldBehavior: " + combo1.EnterFieldBehavior);
            Console.WriteLine("Combo2 EnterFieldBehavior: " + combo2.EnterFieldBehavior);
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


