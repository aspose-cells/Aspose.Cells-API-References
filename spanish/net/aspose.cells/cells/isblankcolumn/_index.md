---
title: "Cells.IsBlankColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Verifica si la columna dada está en blanco y no contiene datos"
type: docs
url: /es/net/aspose.cells/cells/isblankcolumn/
---
## Cells.IsBlankColumn method

Comprueba si la columna dada está vacía (no contiene datos).

```csharp
public bool IsBlankColumn(int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | el índice de columna |

### Valor de retorno

verdadero si la columna dada no contiene datos

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsBlankColumnWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Verificar si la columna 2 está en blanco (debe ser verdadero para una hoja nueva)
            Console.WriteLine("Is column 2 blank? " + worksheet.Cells.IsBlankColumn(1));

            // Agregar datos a la columna 2
            worksheet.Cells["B1"].PutValue("Test Data");

            // Verificar de nuevo (debe ser falso ahora)
            Console.WriteLine("Is column 2 blank after adding data? " + worksheet.Cells.IsBlankColumn(1));

            // Crear otra hoja de cálculo con columnas completamente en blanco
            Worksheet worksheet2 = workbook.Worksheets.Add("BlankSheet");

            // Verificar una columna en la hoja en blanco (debe ser verdadero)
            Console.WriteLine("Is column 3 blank in new sheet? " + worksheet2.Cells.IsBlankColumn(2));
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


