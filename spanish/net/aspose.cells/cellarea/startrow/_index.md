---
title: "CellArea.StartRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Campo CellArea. Obtiene o establece la fila inicial de esta área"
type: docs
url: /es/net/aspose.cells/cellarea/startrow/
---
## CellArea.StartRow field

Obtiene o establece la fila inicial de esta área.

```csharp
public int StartRow;
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear dos objetos CellArea
            CellArea area1 = new CellArea();
            area1.StartRow = 2;
            area1.StartColumn = 1;
            area1.EndRow = 5;
            area1.EndColumn = 3;

            CellArea area2 = new CellArea();
            area2.StartRow = area1.StartRow; // Demonstrating StartRow usage
            area2.StartColumn = area1.StartColumn;
            area2.EndRow = area1.EndRow;
            area2.EndColumn = area1.EndColumn;

            // Verificar que las áreas coincidan
            if (area1.StartRow == area2.StartRow &&
                area1.StartColumn == area2.StartColumn &&
                area1.EndRow == area2.EndRow &&
                area1.EndColumn == area2.EndColumn)
            {
                Console.WriteLine("CellArea objects match successfully");
                Console.WriteLine($"StartRow: {area1.StartRow}");
            }
            else
            {
                Console.WriteLine("CellArea objects do not match");
            }
        }
    }
}
```

### Ver también

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


