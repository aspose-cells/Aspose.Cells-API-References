---
title: "Worksheet.Split"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Divide la ventana"
type: docs
url: /es/net/aspose.cells/worksheet/split/
---
## Worksheet.Split method

Divide la ventana.

```csharp
public void Split()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSplitDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para demostrar la división
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Data " + i);
            }
            
            // Dividir la hoja de cálculo (no se necesitan parámetros)
            worksheet.Split();
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetSplitDemo.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


