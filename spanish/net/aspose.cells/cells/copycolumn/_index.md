---
title: "Cells.CopyColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Copia datos y formatos de una columna completa"
type: docs
url: /es/net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

Copia los datos y formatos de una columna completa.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | Celdas | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceColumnIndex | Int32 | Índice de la columna de origen. |
| destinationColumnIndex | Int32 | Índice de la columna de destino. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Crear libro de origen y poblar datos
            Workbook wbSrc = new Workbook();
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;
            cellsSrc[0, 255].PutValue(1);
            cellsSrc[1, 255].PutValue(true);
            cellsSrc[2, 255].PutValue("abc");
            cellsSrc[3, 255].PutValue(false);
            cellsSrc[65535, 255].PutValue(2.56);

            // Cree un libro de trabajo de destino
            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;

            // Copiar columna del origen al destino
            cellsDest.CopyColumn(cellsSrc, 255, 0);

            // Guardar el resultado
            wbDest.Save("outputCopyColumn.xlsx");
            
            Console.WriteLine("Column copied successfully.");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


