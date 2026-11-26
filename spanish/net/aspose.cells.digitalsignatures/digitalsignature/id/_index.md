---
title: "DigitalSignature.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DigitalSignature. Especifica un GUID que puede cruzarse con el GUID de la línea de firma almacenada en el contenido del documento. El valor predeterminado es GUID vacío de ceros"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/id/
---
## DigitalSignature.Id property

Especifica un GUID que puede ser referenciado cruzadamente con el GUID de la línea de firma almacenada en el contenido del documento. El valor predeterminado es Empty (todos ceros) Guid.

```csharp
public Guid Id { get; set; }
```

### Observaciones

Cuando se establece, asocia [`SignatureLine`](../../../aspose.cells.drawing/signatureline/) con la correspondiente [`DigitalSignature`](../).

### Ejemplos

```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una firma digital con un ID específico
            Guid signatureId = Guid.NewGuid();
            
            // Crear una firma digital
            X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            
            // Establecer el Id de la firma
            signature.Id = signatureId;

            // Agregar firma a la colección
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);

            // Aplicar firma digital al libro de trabajo
            workbook.SetDigitalSignature(dsCollection);

            // Guarda el libro de trabajo
            workbook.Save("signed_workbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


