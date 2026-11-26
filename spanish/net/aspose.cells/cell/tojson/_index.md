---
title: "Cell.ToJson"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Convertir Cell a datos estructurados JSON"
type: docs
url: /es/net/aspose.cells/cell/tojson/
---
## Cell.ToJson method

Convertir [`Cell`](../) a datos estructurados JSON.

```csharp
public string ToJson()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodToJsonDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer datos de muestra y estilos
            cells["A1"].PutValue(100);
            cells["B6"].Formula = "=A1";
            
            // Obtener la celda y convertir a JSON
            Cell cell = cells["B6"];
            string json = cell.ToJson();
            
            // Genera el JSON
            Console.WriteLine("Cell JSON:");
            Console.WriteLine(json);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


