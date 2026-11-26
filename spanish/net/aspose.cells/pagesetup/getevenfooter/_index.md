---
title: "PageSetup.GetEvenFooter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Obtiene un script que formatea el pie de página par de un archivo Excel"
type: docs
url: /es/net/aspose.cells/pagesetup/getevenfooter/
---
## PageSetup.GetEvenFooter method

Obtiene un script que da formato al pie de página par de un archivo Excel.

```csharp
public string GetEvenFooter(int section)
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
    public class PageSetupMethodGetEvenFooterWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Habilitar encabezados/pies de página diferentes para páginas impares y pares
            pageSetup.IsHFDiffOddEven = true;
            
            // Establecer pie de página par
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Obtener y mostrar el pie de página par
            string evenFooter = pageSetup.GetEvenFooter(0);
            Console.WriteLine("Even Footer: " + evenFooter);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


