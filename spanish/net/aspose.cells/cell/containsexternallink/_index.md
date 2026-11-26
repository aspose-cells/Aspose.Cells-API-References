---
title: "Cell.ContainsExternalLink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica si esta celda contiene un enlace externo. Solo se aplica cuando la celda es una celda de fórmula"
type: docs
url: /es/net/aspose.cells/cell/containsexternallink/
---
## Cell.ContainsExternalLink property

Indica si esta celda contiene un enlace externo. Solo se aplica cuando la celda es una celda de fórmula.

```csharp
public bool ContainsExternalLink { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyContainsExternalLinkDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Añade datos de ejemplo y un enlace externo
            sheet.Cells["A1"].PutValue("External Link:");
            sheet.Cells["B1"].Formula = "=HYPERLINK(\"https://www.aspose.com\", \"Aspose\")";
            
            // Comprueba si las celdas contienen enlaces externos
            Console.WriteLine("A1 ContainsExternalLink: " + sheet.Cells["A1"].ContainsExternalLink);
            Console.WriteLine("B1 ContainsExternalLink: " + sheet.Cells["B1"].ContainsExternalLink);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


