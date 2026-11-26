---
title: "PaginatedSaveOptions.IsFontSubstitutionCharGranularity"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con ella"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/
---
## PaginatedSaveOptions.IsFontSubstitutionCharGranularity property

Indica si solo se debe sustituir la fuente del carácter cuando la fuente de la celda no es compatible con él.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Observaciones

El valor predeterminado es false. Primero intentaremos la fuente predeterminada del Libro de trabajo y la de PdfSaveOption/sistema para la fuente de la celda.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIsFontSubstitutionCharGranularityDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Sample Text with Font Substitution");

            XpsSaveOptions saveOptions = new XpsSaveOptions
            {
                IsFontSubstitutionCharGranularity = true,
                DefaultFont = "Arial"
            };

            workbook.Save("FontSubstitutionDemo.xps", saveOptions);
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


