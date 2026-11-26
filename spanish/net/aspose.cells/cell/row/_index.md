---
title: "Cell.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el número de fila cero basado en la celda"
type: docs
url: /es/net/aspose.cells/cell/row/
---
## Cell.Row property

Obtiene el número de fila (basado en cero) de la celda.

```csharp
public int Row { get; }
```

### Property Value

Número de fila de Cell

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra y fórmula
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Buscar celda que contiene la fórmula
            Cell cell = worksheet.Cells.Find("=SUM(A1", null, new FindOptions()
            { 
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains 
            });
            
            // Demostrar la propiedad Row
            Console.WriteLine("Formula found in row: " + cell.Row);
            Console.WriteLine("Formula found in column: " + cell.Column);
            
            // Verificar que la fila sea correcta
            if (cell.Row == 2 && cell.Column == 0)
            {
                Console.WriteLine("Row property works correctly");
            }
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


