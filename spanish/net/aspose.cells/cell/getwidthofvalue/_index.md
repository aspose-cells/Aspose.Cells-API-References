---
title: "Cell.GetWidthOfValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene el ancho del valor en unidades de píxeles"
type: docs
url: /es/net/aspose.cells/cell/getwidthofvalue/
---
## Cell.GetWidthOfValue method

Obtiene el ancho del valor en unidades de píxeles.

```csharp
public int GetWidthOfValue()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetWidthOfValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            cell.PutValue("CellsJava40307");
            int width = cell.GetWidthOfValue();
            
            Console.WriteLine("Width of the cell value: " + width);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


