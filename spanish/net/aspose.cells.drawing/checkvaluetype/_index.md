---
title: "Enum CheckValueType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Drawing.CheckValueType. Representa el tipo de valor de verificación del cuadro de selección"
type: docs
url: /es/net/aspose.cells.drawing/checkvaluetype/
---
## CheckValueType enumeration

Representa el tipo de valor de verificación de la casilla de verificación.

```csharp
public enum CheckValueType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| UnChecked | `0` | UnChecked |
| Checked | `1` | Checked |
| Mixed | `2` | Mixed |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassCheckValueTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar casillas de verificación a la hoja de cálculo
            int checkboxIndex1 = sheet.CheckBoxes.Add(0, 0, 100, 100);
            int checkboxIndex2 = sheet.CheckBoxes.Add(0, 1, 100, 100);

            // Obtener las casillas de verificación y establecer sus propiedades
            Aspose.Cells.Drawing.CheckBox checkbox1 = sheet.CheckBoxes[checkboxIndex1];
            Aspose.Cells.Drawing.CheckBox checkbox2 = sheet.CheckBoxes[checkboxIndex2];

            // Establecer valores de casillas de verificación y estado marcado
            checkbox1.Value = true;
            checkbox1.CheckedValue = CheckValueType.Checked;
            
            checkbox2.Value = false;
            checkbox2.CheckedValue = CheckValueType.UnChecked;  // Note: Changed from Unchecked to UnChecked

            // Vincular casillas de verificación a celdas
            checkbox1.LinkedCell = "A1";
            checkbox2.LinkedCell = "A2";

            // Mostrar los valores de las celdas para demostrar el vínculo
            Console.WriteLine("Cell A1 value (should be true): " + sheet.Cells["A1"].BoolValue);
            Console.WriteLine("Cell A2 value (should be false): " + sheet.Cells["A2"].BoolValue);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


