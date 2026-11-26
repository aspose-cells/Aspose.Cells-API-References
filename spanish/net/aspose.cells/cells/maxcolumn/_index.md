---
title: "Cells.MaxColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Índice de columna máximo de aquellas celdas que se han instanciado en la colección no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella"
type: docs
url: /es/net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

Índice máximo de columna de esas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella).

```csharp
public int MaxColumn { get; }
```

### Observaciones

Devuelve -1 si no se ha instanciado ninguna celda.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["B1"].PutValue("Column B");
            worksheet.Cells["C1"].PutValue("Column C");
            
            // Obtener el índice de columna máximo con datos
            int maxColumn = worksheet.Cells.MaxColumn;
            Console.WriteLine("Max column with data: " + maxColumn);

            // Agregar datos a la siguiente columna después de la columna máxima
            worksheet.Cells[0, maxColumn + 1].PutValue("Next Column");

            // Verificar la nueva columna máxima
            Console.WriteLine("New max column: " + worksheet.Cells.MaxColumn);

            // Crear otra hoja de cálculo para demostrar la copia
            Worksheet destSheet = workbook.Worksheets.Add("Destination");

            // Copiar todas las columnas del origen al destino
            destSheet.Cells.CopyColumns(worksheet.Cells, 0, 0, worksheet.Cells.MaxColumn + 1);

            Console.WriteLine("Columns copied successfully");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


