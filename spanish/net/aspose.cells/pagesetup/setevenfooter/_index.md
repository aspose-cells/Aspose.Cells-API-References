---
title: "PageSetup.SetEvenFooter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Establece un script que formatea el pie de página par de un archivo Excel. Solo tiene efecto en Excel 2007 cuando IsHFDiffOddEven es true"
type: docs
url: /es/net/aspose.cells/pagesetup/setevenfooter/
---
## PageSetup.SetEvenFooter method

Establece un script que da formato al pie de página par de un archivo Excel. Solo tiene efecto en Excel 2007 cuando IsHFDiffOddEven es verdadero.

```csharp
public void SetEvenFooter(int section, string footerScript)
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
    public class PageSetupMethodSetEvenFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Habilitar diferentes encabezados/pies de página para la primera y las páginas pares
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;

            // Establecer diferentes tipos de pie de página
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetFirstPageFooter(0, "First Page Footer");

            // Guarda el libro de trabajo
            workbook.Save("PageSetup_SetEvenFooter_Example.xlsx");

            Console.WriteLine("Workbook saved with even page footer set successfully.");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


