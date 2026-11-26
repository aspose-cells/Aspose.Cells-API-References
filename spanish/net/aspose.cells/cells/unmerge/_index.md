---
title: "Cells.UnMerge"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Descombina un rango especificado de celdas combinadas"
type: docs
url: /es/net/aspose.cells/cells/unmerge/
---
## Cells.UnMerge method

Descombina un rango especificado de celdas combinadas.

```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila de este rango(basado en cero) |
| firstColumn | Int32 | Primera columna de este rango(basado en cero) |
| totalRows | Int32 | Número de filas(basado en uno) |
| totalColumns | Int32 | Número de columnas(basado en uno) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Combina celdas primero
            cells.Merge(0, 0, 2, 2);
            
            // Descombina las celdas previamente combinadas
            cells.UnMerge(0, 0, 2, 2);
            
            // Guarda el libro de trabajo
            workbook.Save("UnMergeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


