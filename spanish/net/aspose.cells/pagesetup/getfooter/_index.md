---
title: "PageSetup.GetFooter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Obtiene un script que formatea el pie de página de un archivo Excel"
type: docs
url: /es/net/aspose.cells/pagesetup/getfooter/
---
## PageSetup.GetFooter method

Obtiene un script que da formato al pie de página de un archivo Excel.

```csharp
public string GetFooter(int section)
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
    public class PageSetupMethodGetFooterWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer diferentes secciones del pie de página
            worksheet.PageSetup.SetFooter(1, "odd");
            worksheet.PageSetup.SetFirstPageFooter(1, "first");
            worksheet.PageSetup.SetEvenFooter(1, "even");

            // Obtener y mostrar las secciones del pie de página
            Console.WriteLine("First Page Footer: " + worksheet.PageSetup.GetFirstPageFooter(1));
            Console.WriteLine("Even Page Footer: " + worksheet.PageSetup.GetEvenFooter(1));
            Console.WriteLine("Odd Page Footer: " + worksheet.PageSetup.GetFooter(1));
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


