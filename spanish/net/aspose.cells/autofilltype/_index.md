---
title: "Enum AutoFillType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.AutoFillType. Representa el tipo de autocompletar"
type: docs
url: /es/net/aspose.cells/autofilltype/
---
## AutoFillType enumeration

Representa el tipo de autocompletar.

```csharp
public enum AutoFillType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Copy | `1` | Copia el valor y el formato del área de origen al área de destino |
| Default | `0` | Llena automáticamente el área de destino con el valor y el formato. |
| Formats | `3` | Copia solo el formato del área de origen al área de destino. |
| Series | `2` | Extiende el valor del área de origen al área de destino en forma de serie y copia el formato al área de destino. |
| Values | `4` | Copia solo el valor del área de origen al área de destino. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFillTypeDemo
    {
        public static void AutoFillTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango (A1:A10) y llenarlo con algunos valores
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A10");
            for (int i = 0; i < 10; i++)
            {
                sourceRange[i, 0].PutValue(i + 1);
            }

            // Crear un rango de destino (B1:B10)
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B10");

            //Error de tipo serie, se ha creado un ticket
            // Utiliza el método AutoFill con AutoFillType.Series para rellenar el rango objetivo
            //sourceRange.AutoFill(targetRange, AutoFillType.Series);

            // Utiliza el método AutoFill con AutoFillType.Copy para rellenar el rango objetivo
            sourceRange.AutoFill(targetRange, AutoFillType.Copy);
            // Guarda el libro de trabajo
            workbook.Save("AutoFillTypeExample.xlsx");
            workbook.Save("AutoFillTypeExample.pdf");
        }
    }

}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


