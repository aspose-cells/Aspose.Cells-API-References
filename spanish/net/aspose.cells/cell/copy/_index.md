---
title: "Cell.Copy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Copia datos de una celda origen"
type: docs
url: /es/net/aspose.cells/cell/copy/
---
## Cell.Copy method

Copia datos de una celda origen.

```csharp
public void Copy(Cell cell)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cell | Cell | Objeto [`Cell`](../) de origen. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCopyWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establezca valores y estilos en la celda origen
            Cell sourceCell = cells["A1"];
            sourceCell.PutValue("Source Value");
            sourceCell.GetStyle().Font.IsBold = true;

            // Cree la celda de destino
            Cell destCell = cells["B1"];

            // Copiar de la celda origen a la celda destino
            destCell.Copy(sourceCell);

            // Verifique la copia
            Console.WriteLine("Destination cell value: " + destCell.StringValue);
            Console.WriteLine("Destination cell bold status: " + destCell.GetStyle().Font.IsBold);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


