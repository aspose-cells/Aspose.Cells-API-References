---
title: "GroupBox.Shadow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GroupBox. Indica si el groupbox tiene sombra"
type: docs
url: /es/net/aspose.cells.drawing/groupbox/shadow/
---
## GroupBox.Shadow property

Indica si el groupbox tiene sombra.

```csharp
public bool Shadow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GroupBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un group box con sombra
            GroupBox groupBoxWithShadow = worksheet.Shapes.AddGroupBox(1, 0, 1, 0, 200, 150);
            groupBoxWithShadow.Shadow = true;
            groupBoxWithShadow.Text = "GroupBox with Shadow";
            
            // Agregar un group box sin sombra
            GroupBox groupBoxWithoutShadow = worksheet.Shapes.AddGroupBox(1, 2, 1, 0, 200, 150);
            groupBoxWithoutShadow.Shadow = false;
            groupBoxWithoutShadow.Text = "GroupBox without Shadow";
            
            // Agregar botones de opción dentro de los group boxes para demostrar la agrupación
            RadioButton radio1 = worksheet.Shapes.AddRadioButton(3, 0, 2, 0, 30, 100);
            radio1.Text = "Option 1";
            radio1.LinkedCell = "A1";
            
            RadioButton radio2 = worksheet.Shapes.AddRadioButton(6, 0, 2, 0, 30, 100);
            radio2.Text = "Option 2";
            radio2.LinkedCell = "A1";
            
            // Agrupar las formas
            Shape[] shapes = { groupBoxWithShadow, radio1, radio2 };
            worksheet.Shapes.Group(shapes);
            
            // Guarda el libro de trabajo
            workbook.Save("GroupBoxShadowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GroupBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


