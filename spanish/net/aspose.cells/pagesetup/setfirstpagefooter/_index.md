---
title: "PageSetup.SetFirstPageFooter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Establece un script que formatea el pie de página de la primera página de un archivo Excel"
type: docs
url: /es/net/aspose.cells/pagesetup/setfirstpagefooter/
---
## PageSetup.SetFirstPageFooter method

Establece un script que da formato al pie de página de la primera hoja de un archivo Excel.

```csharp
public void SetFirstPageFooter(int section, string footerScript)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| footerScript | String | Script de formato de pie de página. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFirstPageFooterWithInt32StringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener el objeto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Establecer encabezados/pies de página diferentes para la primera página
            pageSetup.IsHFDiffFirst = true;
            
            // Establecer el pie de página de la primera página con el índice de sección y texto
            pageSetup.SetFirstPageFooter(0, "First Page Footer Text");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            Console.WriteLine("First page footer set successfully.");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


