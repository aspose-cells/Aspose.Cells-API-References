---
title: "Style.IsDateTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indica si el formato numérico es un formato de fecha"
type: docs
url: /es/net/aspose.cells/style/isdatetime/
---
## Style.IsDateTime property

Indica si el formato numérico es un formato de fecha.

```csharp
public bool IsDateTime { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsDateTimeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Establecer un valor numérico
            cells["A1"].PutValue(1230);
            
            // Obtener y modificar el estilo de la celda
            Style style = cells["A1"].GetStyle();
            
            // Establecer al formato de fecha (15 es el formato de fecha incorporado)
            style.Number = 15;
            Console.WriteLine("IsDateTime after setting Number=15: " + style.IsDateTime);
            
            // Establecer formato de fecha personalizado
            style.Custom = "yyyy-mm-dd";
            Console.WriteLine("IsDateTime after setting custom date format: " + style.IsDateTime);
            
            // Aplicar el estilo modificado a la celda
            cells["A1"].SetStyle(style);
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


