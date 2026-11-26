---
title: "Range.GetCellOrNull"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Obtiene el objeto Cell o null en este rango"
type: docs
url: /es/net/aspose.cells/range/getcellornull/
---
## Range.GetCellOrNull method

Obtiene el objeto [`Cell`](../../cell/) o null en este rango.

```csharp
public Cell GetCellOrNull(int rowOffset, int columnOffset)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | Int32 | Desplazamiento de fila en este rango, basado en cero. |
| columnOffset | Int32 | Desplazamiento de columna en este rango, basado en cero. |

### Valor de retorno

[`Cell`](../../cell/) object.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetCellOrNullWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree un rango
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            
            // Rellene algunos datos en el rango
            range[0, 0].PutValue("Cell A1");
            range[0, 1].PutValue("Cell B1");
            range[1, 0].PutValue("Cell A2");
            
            // Demuestre GetCellOrNull con parámetros Int32
            Cell cell1 = range.GetCellOrNull(0, 0);
            Console.WriteLine("Cell (0,0): " + (cell1 != null ? cell1.StringValue : "null"));
            
            Cell cell2 = range.GetCellOrNull(1, 1);
            Console.WriteLine("Cell (1,1): " + (cell2 != null ? cell2.StringValue : "null"));
            
            // Intente obtener una celda fuera del rango (debe devolver null)
            Cell cell3 = range.GetCellOrNull(2, 0);
            Console.WriteLine("Cell (2,0): " + (cell3 != null ? cell3.StringValue : "null"));
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


