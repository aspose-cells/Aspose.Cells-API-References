---
title: "PageSetup.GetHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Obtiene un script que formatea el encabezado de un archivo Excel"
type: docs
url: /es/net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

Obtiene un script que da formato al encabezado de un archivo Excel.

```csharp
public string GetHeader(int section)
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
    public class PageSetupMethodGetHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establezca el encabezado para la sección 2
            worksheet.PageSetup.SetHeader(2, "&8Report ID: TEST01\n你好Public");
            
            // Obtenga e imprima el encabezado para la sección 2
            string header = worksheet.PageSetup.GetHeader(2);
            Console.WriteLine("Header for section 2: " + header);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


