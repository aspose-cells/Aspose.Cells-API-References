---
title: "OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsLoadOptions. Indica si se aplica el estilo predeterminado de Excel al hipervínculo"
type: docs
url: /es/net/aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/
---
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property

Indica si se aplica el estilo predeterminado de Excel al hipervínculo.

```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyApplyExcelDefaultStyleToHyperlinkDemo
    {
        public static void Run()
        {
            // Crea una instancia de OdsLoadOptions
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // Establecer la propiedad ApplyExcelDefaultStyleToHyperlink
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            // Carga un archivo ODS con las opciones especificadas
            Workbook workbook = new Workbook("sample.ods", loadOptions);

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un hipervínculo para demostrar la aplicación del estilo
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Guardar el libro de trabajo en un archivo nuevo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


