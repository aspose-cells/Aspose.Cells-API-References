---
title: "SignatureLine.IsLine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SignatureLine. Indica si es una línea de firma"
type: docs
url: /es/net/aspose.cells.drawing/signatureline/isline/
---
## SignatureLine.IsLine property

Indica si es una línea de firma.

```csharp
public bool IsLine { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIsLineDemo
    {
        public static void Run()
        {
            // Crear una instancia de línea de firma
            SignatureLine signature = new SignatureLine();
            
            // Establecer IsLine a true
            signature.IsLine = true;
            
            // Comprobar y demostrar el uso de IsLine
            if (signature.IsLine)
            {
                Console.WriteLine("Signature line is active.");
            }
            
            // Alternar el estado de IsLine
            signature.IsLine = false;
            
            if (!signature.IsLine)
            {
                Console.WriteLine("Signature line is now inactive.");
            }
        }
    }
}
```

### Ver también

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


