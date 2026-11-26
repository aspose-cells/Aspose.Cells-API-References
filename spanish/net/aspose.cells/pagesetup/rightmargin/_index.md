---
title: "PageSetup.RightMargin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el tamaño del margen derecho en unidades de centímetros"
type: docs
url: /es/net/aspose.cells/pagesetup/rightmargin/
---
## PageSetup.RightMargin property

Representa el tamaño del margen derecho, en unidades de centímetros.

```csharp
public double RightMargin { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer diferentes márgenes derechos y guardar para demostrar el efecto
            worksheet.PageSetup.RightMargin = 0;
            workbook.Save("RightMargin_0.xlsx");

            worksheet.PageSetup.RightMargin = 1.0;
            workbook.Save("RightMargin_1.xlsx");

            worksheet.PageSetup.RightMargin = 2.5;
            workbook.Save("RightMargin_2.5.xlsx");

            // Imprimir el valor actual del margen derecho
            Console.WriteLine("Current Right Margin: " + worksheet.PageSetup.RightMargin);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


