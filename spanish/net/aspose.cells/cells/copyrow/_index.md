---
title: "Cells.CopyRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Copia los datos y formatos de una fila completa"
type: docs
url: /es/net/aspose.cells/cells/copyrow/
---
## Cells.CopyRow method

Copia los datos y formatos de una fila completa.

```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceCells | Celdas | El objeto Source Cells contiene datos y formatos para copiar. |
| sourceRowIndex | Int32 | Índice de fila de origen. |
| destinationRowIndex | Int32 | Índice de fila de destino. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet1 = workbook.Worksheets[0];
            Cells cells1 = worksheet1.Cells;
            
            // Agregar algunos datos a la primera fila
            cells1["A1"].PutValue("Source Data");
            cells1["B1"].PutValue(100);
            cells1["C1"].PutValue(DateTime.Now);
            
            // Crear segunda hoja de cálculo
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            Cells cells2 = worksheet2.Cells;
            
            // Copiar fila de Sheet1 a Sheet2
            cells2.CopyRow(cells1, 0, 0);
            
            // Copiar fila dentro de Sheet1 a nuevas posiciones
            cells1.CopyRow(cells1, 0, 1);
            cells1.CopyRow(cells1, 0, 2);
            
            // Guarda el libro de trabajo
            workbook.Save("CopyRowExample.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


