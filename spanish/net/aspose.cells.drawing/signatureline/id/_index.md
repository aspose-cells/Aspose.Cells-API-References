---
title: "SignatureLine.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SignatureLine. Obtiene o establece el identificador de esta línea de firma"
type: docs
url: /es/net/aspose.cells.drawing/signatureline/id/
---
## SignatureLine.Id property

Obtiene o establece el identificador de esta línea de firma.

```csharp
public Guid Id { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un objeto de línea de firma
            SignatureLine signatureLine = new SignatureLine();
            Guid signatureId = Guid.NewGuid();
            signatureLine.Id = signatureId;
            
            // Agregar la línea de firma a la hoja de cálculo en la posición (1,1)
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Mostrar el ID de la línea de firma
            Console.WriteLine("Signature Line ID: " + signatureLine.Id);
        }
    }
}
```

### Ver también

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


