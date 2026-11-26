---
title: "ActiveXControl.IMEMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ActiveXControl. Obtiene y establece el modo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrol/imemode/
---
## ActiveXControl.IMEMode property

Obtiene y establece el modo de tiempo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco.

```csharp
public InputMethodEditorMode IMEMode { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIMEModeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ToggleButton con coordenadas adecuadas
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 
                1, 1,  // Upper-left row/column
                1, 1,  // Upper-left row/column offsets
                100, 50);  // Width and height
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Establecer propiedades incluyendo IMEMode
            toggleButton.Caption = "ToggleButton1";
            toggleButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            toggleButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            toggleButton.IMEMode = InputMethodEditorMode.NoControl;

            // Verificar y mostrar la propiedad IMEMode
            Console.WriteLine("ToggleButton IMEMode: " + toggleButton.IMEMode);

            // Guarda el libro de trabajo
            workbook.Save("ActiveXControlIMEModeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [InputMethodEditorMode](../../inputmethodeditormode/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


