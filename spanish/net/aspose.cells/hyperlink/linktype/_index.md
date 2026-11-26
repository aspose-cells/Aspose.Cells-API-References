---
title: "Hyperlink.LinkType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Hyperlink. Obtiene el tipo de enlace"
type: docs
url: /es/net/aspose.cells/hyperlink/linktype/
---
## Hyperlink.LinkType property

Obtiene el tipo de enlace.

```csharp
public TargetModeType LinkType { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyLinkTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un hipervínculo externo
            int hyperlinkIndex = worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            Hyperlink link = worksheet.Hyperlinks[hyperlinkIndex];
            
            // Demostrar la propiedad LinkType
            Console.WriteLine("Hyperlink LinkType: " + link.LinkType);
            
            // Limpiar
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Ver también

* enum [TargetModeType](../../targetmodetype/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


