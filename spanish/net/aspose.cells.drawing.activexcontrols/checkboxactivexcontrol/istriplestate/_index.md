---
title: "CheckBoxActiveXControl.IsTripleState"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CheckBoxActiveXControl. Indica cómo el control especificado mostrará valores nulos"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/istriplestate/
---
## CheckBoxActiveXControl.IsTripleState property

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
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control CheckBox ActiveX con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Configurar propiedades básicas
            checkBox.Caption = "Triple State Demo";
            
            // Demostrar la propiedad IsTripleState
            checkBox.IsTripleState = true; // Enable three states: Checked, Unchecked, and Indeterminate
            checkBox.Value = CheckValueType.Mixed; // Set to indeterminate state

            // Guarda el libro de trabajo
            workbook.Save("CheckBoxTripleStateDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


