---
title: "Font.DoubleSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene y establece el tamaño doble de la fuente"
type: docs
url: /es/net/aspose.cells/font/doublesize/
---
## Font.DoubleSize property

Obtiene y establece el doble tamaño de la fuente.

```csharp
public double DoubleSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyDoubleSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.Font.DoubleSize = 10.5;
            cell.SetStyle(style);
            
            Console.WriteLine("Font DoubleSize set to: " + cell.GetStyle().Font.DoubleSize);
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


