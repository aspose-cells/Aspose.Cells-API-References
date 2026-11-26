---
title: "PageSetup.SetEvenHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Establece un script que formatea el encabezado de página par de un archivo Excel. Solo tiene efecto en Excel 2007 cuando IsHFDiffOddEven es verdadero"
type: docs
url: /es/net/aspose.cells/pagesetup/setevenheader/
---
## PageSetup.SetEvenHeader method

Establece un script que da formato al encabezado par de un archivo Excel. Solo tiene efecto en Excel 2007 cuando IsHFDiffOddEven es verdadero.

```csharp
public void SetEvenHeader(int section, string headerScript)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| headerScript | String | Script de formato de encabezado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Habilitar encabezados/pies de página diferentes para páginas impares y pares
            pageSetup.IsHFDiffOddEven = true;

            // Establecer el encabezado de página par con índice de sección y texto
            pageSetup.SetEvenHeader(1, "Even Page Header - Center Section");
            pageSetup.SetEvenHeader(0, "Even Page Header - Left Section");
            pageSetup.SetEvenHeader(2, "Even Page Header - Right Section");

            // Guarda el libro de trabajo
            workbook.Save("PageSetup_SetEvenHeaderExample.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


