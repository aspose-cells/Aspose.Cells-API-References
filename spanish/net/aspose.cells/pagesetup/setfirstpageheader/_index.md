---
title: "PageSetup.SetFirstPageHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Establece un script que formatea el encabezado de la primera página de un archivo Excel. Solo tiene efecto en Excel 2007 cuando IsHFDiffFirst es verdadero"
type: docs
url: /es/net/aspose.cells/pagesetup/setfirstpageheader/
---
## PageSetup.SetFirstPageHeader method

Establece un script que da formato al encabezado de la primera página de un archivo de Excel. Solo tiene efecto en Excel 2007 cuando IsHFDiffFirst es verdadero.

```csharp
public void SetFirstPageHeader(int section, string headerScript)
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
    public class PageSetupMethodSetFirstPageHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer el encabezado de la primera página con número de sección y texto del encabezado
            pageSetup.SetFirstPageHeader(2, "&CHeader Text");

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


