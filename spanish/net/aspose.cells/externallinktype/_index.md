---
title: "Enumeración ExternalLinkType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.ExternalLinkType. Representa el tipo de enlace externo"
type: docs
url: /es/net/aspose.cells/externallinktype/
---
## ExternalLinkType enumeration

Representa el tipo de enlace externo.

```csharp
public enum ExternalLinkType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DDELink | `0` | Representa el enlace DDE. |
| External | `1` | Representa un enlace externo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkTypeDemo
    {
        public static void ExternalLinkTypeExample()
        {
            // Abrir un archivo con enlaces externos
            Workbook workbook = new Workbook("ExternalLinkTypeExample_original.xlsx");

            // Obtener enlace externo 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Mostrar el tipo de enlace externo
            Console.WriteLine("External Link Type: " + externalLink.Type);

            // Cambiar la fuente de datos del enlace externo
            externalLink.DataSource = "d:\\link.xls";

            // Guarda el libro de trabajo
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }

    // Enumeración que representa el tipo de enlace externo
    public enum ExternalLinkType
    {
        DDELink = 0, // Represents the DDE link
        External = 1 // Represents external link
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


