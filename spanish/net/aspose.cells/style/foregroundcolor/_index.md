---
title: "Style.ForegroundColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene o establece el color de primer plano de un estilo"
type: docs
url: /es/net/aspose.cells/style/foregroundcolor/
---
## Style.ForegroundColor property

Obtiene o establece el color de primer plano de un estilo.

```csharp
public Color ForegroundColor { get; set; }
```

### Observaciones

Significa que no hay configuración de color si se devuelve Color.Empty.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Green;
            style.Pattern = BackgroundType.Solid;
            
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            Console.WriteLine("ForegroundColor set to: " + style.ForegroundColor);
            
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


