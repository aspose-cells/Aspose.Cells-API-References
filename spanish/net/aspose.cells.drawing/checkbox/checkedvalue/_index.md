---
title: "CheckBox.CheckedValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CheckBox. Obtiene o establece el valor de la casilla de verificación"
type: docs
url: /es/net/aspose.cells.drawing/checkbox/checkedvalue/
---
## CheckBox.CheckedValue property

Obtiene o establece el valor del checkbox.

```csharp
public CheckValueType CheckedValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyCheckedValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar un checkbox a la hoja de cálculo
            CheckBox checkBox = sheet.Shapes.AddCheckBox(1, 1, 100, 100, 20, 20);

            // Establecer el valor de la casilla de verificación a Marcado
            checkBox.CheckedValue = CheckValueType.Checked;

            // Guarda el libro de trabajo
            workbook.Save("CheckBoxCheckedValueDemo.xlsx");

            // Cargar el libro de trabajo guardado para verificar
            Workbook loadedWorkbook = new Workbook("CheckBoxCheckedValueDemo.xlsx");
            CheckBox loadedCheckBox = (CheckBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Mostrar el estado de la casilla de verificación
            Console.WriteLine("CheckBox CheckedValue: " + loadedCheckBox.CheckedValue);
        }
    }
}
```

### Ver también

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


