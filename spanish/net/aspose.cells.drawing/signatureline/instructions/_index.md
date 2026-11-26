---
title: "SignatureLine.Instructions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SignatureLine. Obtiene o establece el texto mostrado al usuario al firmar"
type: docs
url: /es/net/aspose.cells.drawing/signatureline/instructions/
---
## SignatureLine.Instructions property

Obtiene o establece el texto mostrado al usuario al firmar.

```csharp
public string Instructions { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyInstructionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un objeto de línea de firma
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Instructions = "Please sign here after reviewing the document.";

            // Agregar la línea de firma a la hoja de cálculo en la posición (1,1)
            worksheet.Shapes.AddSignatureLine(1, 1, signatureLine);

            // Guarda el libro de trabajo
            workbook.Save("SignatureLineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


