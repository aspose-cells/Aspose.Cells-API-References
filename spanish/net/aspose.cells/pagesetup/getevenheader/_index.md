---
title: "PageSetup.GetEvenHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Obtiene un script que formatea el encabezado par de un archivo Excel"
type: docs
url: /es/net/aspose.cells/pagesetup/getevenheader/
---
## PageSetup.GetEvenHeader method

Obtiene un script que da formato al encabezado par de un archivo Excel.

```csharp
public string GetEvenHeader(int section)
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
    public class PageSetupMethodGetEvenHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Habilitar encabezados/pies de página diferentes para pares e impares
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.IsHFDiffOddEven = true;
            
            // Establecer encabezado de página par
            pageSetup.SetEvenHeader(0, "&CEven Page Header Center");
            pageSetup.SetEvenHeader(1, "&LEven Page Header Left");
            pageSetup.SetEvenHeader(2, "&REven Page Header Right");
            
            // Obtener e imprimir encabezados de página pares
            Console.WriteLine("Even Header Center: " + pageSetup.GetEvenHeader(0));
            Console.WriteLine("Even Header Left: " + pageSetup.GetEvenHeader(1));
            Console.WriteLine("Even Header Right: " + pageSetup.GetEvenHeader(2));
            
            // Guarda el libro de trabajo
            workbook.Save("PageSetup_GetEvenHeaderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


