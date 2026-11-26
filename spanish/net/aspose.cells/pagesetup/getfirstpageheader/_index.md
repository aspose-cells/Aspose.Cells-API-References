---
title: "PageSetup.GetFirstPageHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Obtiene un script que formatea el encabezado de la primera página de un archivo Excel"
type: docs
url: /es/net/aspose.cells/pagesetup/getfirstpageheader/
---
## PageSetup.GetFirstPageHeader method

Obtiene un script que da formato al encabezado de la primera hoja de un archivo Excel.

```csharp
public string GetFirstPageHeader(int section)
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
    public class PageSetupMethodGetFirstPageHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Habilitar encabezado/pie de página diferente en la primera página
            pageSetup.IsHFDiffFirst = true;
            
            // Establecer secciones del encabezado de la primera página
            pageSetup.SetFirstPageHeader(0, "&LFirst Page Left Header");
            pageSetup.SetFirstPageHeader(1, "&CFirst Page Center Header");
            pageSetup.SetFirstPageHeader(2, "&RFirst Page Right Header");
            
            // Obtener y mostrar secciones del encabezado de la primera página
            Console.WriteLine("First Page Header Sections:");
            Console.WriteLine("Left: " + pageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Center: " + pageSetup.GetFirstPageHeader(1));
            Console.WriteLine("Right: " + pageSetup.GetFirstPageHeader(2));
            
            // Guarda el libro de trabajo
            workbook.Save("PageSetupFirstPageHeaderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


