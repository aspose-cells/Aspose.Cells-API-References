---
title: "ActiveXControl.IsLocked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ActiveXControl. Indica si los datos del control están bloqueados para edición"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrol/islocked/
---
## ActiveXControl.IsLocked property

Indica si los datos del control están bloqueados para edición.

```csharp
public bool IsLocked { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsLockedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Desbloquear todas las columnas excepto la primera
            Style style;
            StyleFlag flag;
            for (int i = 0; i <= 255; i++)
            {
                style = sheet.Cells.Columns[(byte)i].GetStyle();
                style.IsLocked = false;
                flag = new StyleFlag();
                flag.Locked = true;
                sheet.Cells.Columns[(byte)i].ApplyStyle(style, flag);
            }

            // Bloquear la primera columna
            style = sheet.Cells.Columns[0].GetStyle();
            style.IsLocked = true;
            flag = new StyleFlag();
            flag.Locked = true;
            sheet.Cells.Columns[0].ApplyStyle(style, flag);

            // Agregar control ActiveX ComboBox
            Shape comboBoxShape = sheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                5, 0, 5, 0, 100, 20);

            // Establecer propiedades del control ActiveX incluyendo IsLocked
            ComboBoxActiveXControl comboBox = 
                (ComboBoxActiveXControl)comboBoxShape.ActiveXControl;
            comboBox.IsLocked = false; // Demonstrate IsLocked property
            comboBox.IsVisible = true;
            comboBox.BorderStyle = ControlBorderType.None;

            // Proteger la hoja de cálculo
            sheet.Protect(ProtectionType.All);

            // Guarda el libro de trabajo
            wb.Save("ActiveXControlIsLockedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


