---
title: "Cells.MinDataColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Índice de columna mínimo de la celda que contiene datos"
type: docs
url: /es/net/aspose.cells/cells/mindatacolumn/
---
## Cells.MinDataColumn property

Índice mínimo de columna de la celda que contiene datos.

```csharp
public int MinDataColumn { get; }
```

### Observaciones

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Agregar algunos datos a las celdas (comenzando desde la columna 2)
            cells["B1"].PutValue("Header1");
            cells["C2"].PutValue("Data1");
            cells["D3"].PutValue("Data2");
            cells["E4"].PutValue("Data3");
            
            // Obtener el índice de columna mínimo que contiene datos
            int minDataColumn = cells.MinDataColumn;
            
            // Mostrar el resultado
            Console.WriteLine("Minimum data column index: " + minDataColumn);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


