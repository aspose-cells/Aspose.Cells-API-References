---
title: "ToggleButtonActiveXControl.IsTripleState"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ToggleButtonActiveXControl. Indica cómo el control especificado mostrará valores nulos"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/istriplestate/
---
## ToggleButtonActiveXControl.IsTripleState property

Indica cómo el control especificado mostrará valores Null.

```csharp
public bool IsTripleState { get; set; }
```

### Observaciones

| **Configuración** | **Description** |
| --- | --- |
| True | El control ciclará a través de los estados para los valores Sí, No y Nulo. El control aparece atenuado (grisáceo) cuando su propiedad Value se establece en Nulo. |
| False | (Predeterminado) El control ciclará a través de los estados para los valores Sí y No. Los valores nulos se muestran como si fueran valores No. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ToggleButton
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 0, 1, 0, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Establezca la propiedad IsTripleState en true
            toggleButton.IsTripleState = true;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Cambie la propiedad IsTripleState a false
            toggleButton.IsTripleState = false;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Guarda el libro de trabajo
            workbook.Save("ToggleButtonIsTripleStateDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


