---
title: "Style.ToJson"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Convertir Style a datos estructurados JSON"
type: docs
url: /es/net/aspose.cells/style/tojson/
---
## Style.ToJson method

Convertir [`Style`](../) a datos estructurados JSON.

```csharp
public string ToJson()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodToJsonDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear y aplicar un estilo a la celda B4
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Yellow;
            cells["B4"].SetStyle(style);

            // Convertir estilo a JSON
            string styleJson = style.ToJson();
            Console.WriteLine("Style JSON:");
            Console.WriteLine(styleJson);

            // Establezca la fórmula en la celda B6
            cells["B6"].Formula = "=A1";

            // Convertir celda a JSON
            string cellJson = cells["B6"].ToJson();
            Console.WriteLine("\nCell JSON:");
            Console.WriteLine(cellJson);
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


