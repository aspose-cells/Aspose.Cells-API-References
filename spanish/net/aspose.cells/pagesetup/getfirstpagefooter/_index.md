---
title: "PageSetup.GetFirstPageFooter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Obtiene un script que formatea el pie de página de la primera página de un archivo Excel"
type: docs
url: /es/net/aspose.cells/pagesetup/getfirstpagefooter/
---
## PageSetup.GetFirstPageFooter method

Obtiene un script que da formato al pie de página de la primera hoja de un archivo Excel.

```csharp
public string GetFirstPageFooter(int section)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetFirstPageFooterWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer el pie de página de la primera página
            worksheet.PageSetup.SetFirstPageFooter(1, "First Page Footer");

            // Obtener e imprimir el pie de página de la primera página
            string footer = worksheet.PageSetup.GetFirstPageFooter(1);
            Console.WriteLine("First Page Footer: " + footer);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


