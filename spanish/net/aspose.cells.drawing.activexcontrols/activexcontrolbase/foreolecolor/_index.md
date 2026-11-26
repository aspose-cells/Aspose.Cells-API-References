---
title: "ActiveXControlBase.ForeOleColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Obtiene y establece el color ole del primer plano"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/
---
## ActiveXControlBase.ForeOleColor property

Obtiene y establece el color OLE del primer plano.

```csharp
public virtual int ForeOleColor { get; set; }
```

### Observaciones

No se aplica al control Image.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyForeOleColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control CheckBox ActiveX con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades básicas
            checkBox.Caption = "Sample CheckBox";
            checkBox.IsAutoSize = true;

            // Demostrar la propiedad ForeOleColor
            checkBox.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            checkBox.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);

            // Guarda el libro de trabajo
            workbook.Save("ActiveXControlForeOleColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


