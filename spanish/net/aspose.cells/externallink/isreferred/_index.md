---
title: "ExternalLink.IsReferred"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalLink. Indica si este enlace externo es referenciado por otros"
type: docs
url: /es/net/aspose.cells/externallink/isreferred/
---
## ExternalLink.IsReferred property

Indica si este enlace externo es referenciado por otros.

```csharp
public bool IsReferred { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsReferredDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con enlace externo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar referencia de enlace externo
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Verifique si el enlace externo está referenciado
            if (workbook.Worksheets.ExternalLinks.Count > 0)
            {
                bool isReferred = workbook.Worksheets.ExternalLinks[0].IsReferred;
                Console.WriteLine("Is external link referred: " + isReferred);
            }
        }
    }
}
```

### Ver también

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


