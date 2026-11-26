---
title: "SignatureLine.Title"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SignatureLine. Obtiene o establece el título del firmante"
type: docs
url: /es/net/aspose.cells.drawing/signatureline/title/
---
## SignatureLine.Title property

Obtiene o establece el título del cantante.

```csharp
public string Title { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyTitleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una línea de firma y establecer su título
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Title = "Development Lead";

            // Agregar la línea de firma a las formas de la hoja de cálculo con parámetros de posición
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Mostrar el título para demostrar que la propiedad fue establecida
            Console.WriteLine("Signature Line Title: " + signatureLine.Title);
        }
    }
}
```

### Ver también

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


