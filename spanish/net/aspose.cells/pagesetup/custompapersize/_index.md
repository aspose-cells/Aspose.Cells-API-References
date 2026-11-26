---
title: "PageSetup.CustomPaperSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Establece el tamaño de papel personalizado en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/pagesetup/custompapersize/
---
## PageSetup.CustomPaperSize method

Establece el tamaño de papel personalizado, en unidades de pulgadas.

```csharp
public void CustomPaperSize(double width, double height)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ancho | Double | El ancho del papel. |
| altura | Double | La altura del papel. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCustomPaperSizeWithDoubleDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer tamaño de papel personalizado (ancho: 1.5 pulgadas, altura: 1.5 pulgadas)
            worksheet.PageSetup.CustomPaperSize(1.5, 1.5);
            
            // Guarda el libro de trabajo para demostrar el efecto
            workbook.Save("CustomPaperSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


