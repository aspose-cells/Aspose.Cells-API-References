---
title: "JsonSaveOptions.Indent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Indica la sangría"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/indent/
---
## JsonSaveOptions.Indent property

Indica la sangría.

```csharp
public string Indent { get; set; }
```

### Observaciones

Si la sangría es nula o vacía, el JSON exportado no está formateado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Configura las opciones de guardado JSON con sangría
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                Indent = "    ", // 4 spaces for indentation
                ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Guardar con salida JSON con sangría
            workbook.Save("IndentedJsonOutput.json", saveOptions);
        }
    }
}
```

### Ver también

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


