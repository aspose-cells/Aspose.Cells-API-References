---
title: "SignatureLine.ProviderId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SignatureLine. Obtiene o establece el id del proveedor de firmas"
type: docs
url: /es/net/aspose.cells.drawing/signatureline/providerid/
---
## SignatureLine.ProviderId property

Obtiene o establece el id del proveedor de firma.

```csharp
public Guid ProviderId { get; set; }
```

### Observaciones

Normalmente es el CLSID del complemento COM del proveedor.

### Ejemplos

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyProviderIdDemo
    {
        public static void Run()
        {
            // Crear una nueva línea de firma
            SignatureLine signatureLine = new SignatureLine();
            
            // Establecer propiedades de la línea de firma
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";
            signatureLine.IsLine = true;
            
            // Establecer ID del proveedor (GUID de ejemplo - debe reemplazarse con el GUID real del proveedor)
            signatureLine.ProviderId = new Guid("000CD6A4-0000-0000-C000-000000000046");
            
            // Establecer tipo de firma (esto debe coincidir con el ID del proveedor)
            signatureLine.SignatureLineType = SignatureType.Stamp;
            
            // Mostrar el ID del proveedor para demostrar su uso
            Console.WriteLine("Signature Line Provider ID: " + signatureLine.ProviderId);
        }
    }
}
```

### Ver también

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


