---
title: "CheckBox.Shadow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CheckBox. Indica si la casilla de verificación tiene sombreado 3D"
type: docs
url: /es/net/aspose.cells.drawing/checkbox/shadow/
---
## CheckBox.Shadow property

Indica si el cuadro combinado tiene sombreado 3D.

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
    public class CheckBoxPropertyShadowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar una casilla de verificación a la hoja de cálculo y obtener su índice
            int checkBoxIndex = sheet.CheckBoxes.Add(1, 1, 20, 100);
            CheckBox checkBox = sheet.CheckBoxes[checkBoxIndex];
            
            // Configurar propiedades de la casilla de verificación
            checkBox.Text = "Enable Feature";
            checkBox.Value = true;
            
            // Demostrar la propiedad Shadow
            checkBox.Shadow = true; // Enable shadow effect
            workbook.Save("CheckBoxWithShadow.xlsx");
            
            checkBox.Shadow = false; // Disable shadow effect
            workbook.Save("CheckBoxWithoutShadow.xlsx");
        }
    }
}
```

### Ver también

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


