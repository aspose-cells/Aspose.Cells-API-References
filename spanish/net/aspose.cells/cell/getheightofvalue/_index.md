---
title: "Cell.GetHeightOfValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene la altura del valor en unidad de píxeles"
type: docs
url: /es/net/aspose.cells/cell/getheightofvalue/
---
## Cell.GetHeightOfValue method

Obtiene la altura del valor en unidades de píxeles.

```csharp
public int GetHeightOfValue()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHeightOfValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer valor y medir la altura
            worksheet.Cells["A1"].PutValue("Sample Text");
            double height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height of value in A1: " + height);
            
            // Ajustar la altura de la fila y medir de nuevo
            worksheet.Cells.Rows[0].Height = 30;
            height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height after row adjustment: " + height);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


