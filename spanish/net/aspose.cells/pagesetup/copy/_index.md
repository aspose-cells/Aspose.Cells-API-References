---
title: "PageSetup.Copy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Copia la configuración del diseño de página"
type: docs
url: /es/net/aspose.cells/pagesetup/copy/
---
## PageSetup.Copy method

Copia la configuración de la configuración de página.

```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | PageSetup | La fuente. |
| copyOptions | CopyOptions | Las opciones de copia. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCopyWithPageSetupCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Establece las propiedades de PageSetup para la primera hoja de cálculo
            workbook.Worksheets[0].PageSetup.PaperSize = PaperSizeType.PaperA3;
            
            // Copia PageSetup de la primera hoja de cálculo a la segunda hoja de cálculo con CopyOptions
            workbook.Worksheets[1].PageSetup.Copy(workbook.Worksheets[0].PageSetup, new CopyOptions());
            
            Console.WriteLine("Paper size of second worksheet: " + workbook.Worksheets[1].PageSetup.PaperSize);
        }
    }
}
```

### Ver también

* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


