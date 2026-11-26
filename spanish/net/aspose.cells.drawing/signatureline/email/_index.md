---
title: "SignatureLine.Email"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SignatureLine. Obtiene o establece el correo electrónico del firmante"
type: docs
url: /es/net/aspose.cells.drawing/signatureline/email/
---
## SignatureLine.Email property

Obtiene o establece el correo electrónico del cantante.

```csharp
public string Email { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyEmailDemo
    {
        public static void Run()
        {
            // Crear una nueva línea de firma
            SignatureLine signatureLine = new SignatureLine();
            
            // Establecer propiedades de la línea de firma incluyendo Email
            signatureLine.Signer = "Simon Zhao";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "Simon.Zhao@aspose.com";
            signatureLine.IsLine = true;
            signatureLine.ShowSignedDate = true;
            
            // Mostrar la propiedad Email
            Console.WriteLine("Signer Email: " + signatureLine.Email);
        }
    }
}
```

### Ver también

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


