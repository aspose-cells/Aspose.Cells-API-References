---
title: "Cells.InsertRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Inserta una nueva fila en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/insertrow/
---
## Cells.InsertRow method

Inserta una nueva fila en la hoja de cálculo.

```csharp
public void InsertRow(int rowIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de fila. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Obtener colección de celdas
            Cells cells = sheet.Cells;
            
            // Inserte datos de ejemplo en la fila 6
            cells[6, 0].PutValue("Original Row 6");
            cells[6, 1].PutValue(100);
            
            // Inserte datos de ejemplo en la fila 7
            cells[7, 0].PutValue("Original Row 7");
            cells[7, 1].PutValue(200);
            
            // Inserte una nueva fila en el índice 7 (desplaza la fila 7 existente hacia abajo)
            cells.InsertRow(7);
            
            // Agregue datos a la fila recién insertada
            cells[7, 0].PutValue("New Inserted Row");
            cells[7, 1].PutValue(150);
            
            // Guarda el libro de trabajo
            workbook.Save("InsertRowDemo.xlsx");
            
            Console.WriteLine("Row inserted successfully at index 7.");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


