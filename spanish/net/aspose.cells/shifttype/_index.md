---
title: "Enumeración ShiftType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ShiftType enum. Representa las opciones de desplazamiento al eliminar un rango de celdas"
type: docs
url: /es/net/aspose.cells/shifttype/
---
## ShiftType enumeration

Representa las opciones de desplazamiento al eliminar un rango de celdas.

```csharp
public enum ShiftType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Down | `0` | Desplazar celdas hacia abajo. |
| Left | `1` | Desplazar celdas a la izquierda. |
| None | `2` | No desplazar celdas. |
| Right | `3` | Desplazar celdas a la derecha. |
| Up | `4` | Desplazar celdas hacia arriba. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ShiftTypeDemo
    {
        public static void ShiftTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Insertar una nueva fila en el índice 1, desplazando las filas existentes hacia abajo
            worksheet.Cells.InsertRows(1, 1, true);

            // Establecer un valor en la fila recién insertada
            worksheet.Cells["A1"].PutValue("New Item");

            // Eliminar un rango de celdas y desplazar las celdas hacia arriba
            worksheet.Cells.DeleteRange(2, 0, 2, 1, ShiftType.Up);

            // Mostrar los valores restantes en la primera columna
            for (int row = 0; row < worksheet.Cells.MaxDataRow + 1; row++)
            {
                Console.WriteLine(worksheet.Cells[row, 0].StringValue);
            }

            // Guarda el libro de trabajo
            workbook.Save("ShiftTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


