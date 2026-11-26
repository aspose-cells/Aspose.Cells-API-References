---
title: "SpreadsheetML2003SaveOptions.IsIndentedFormatting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SpreadsheetML2003SaveOptions. Hace que los elementos secundarios se sangren"
type: docs
url: /es/net/aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/
---
## SpreadsheetML2003SaveOptions.IsIndentedFormatting property

Hace que los elementos secundarios se sangren.

```csharp
public bool IsIndentedFormatting { get; set; }
```

### Observaciones

El valor predeterminado es true. Si el valor es false, reducirá el tamaño del archivo xml

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyIsIndentedFormattingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Configura las opciones de guardado con sangrado
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions
            {
                IsIndentedFormatting = true
            };

            // Guardar con formato XML sangrado
            workbook.Save("output_indented.xml", saveOptions);

            // Guardar sin sangría para comparación
            saveOptions.IsIndentedFormatting = false;
            workbook.Save("output_not_indented.xml", saveOptions);
        }
    }
}
```

### Ver también

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


