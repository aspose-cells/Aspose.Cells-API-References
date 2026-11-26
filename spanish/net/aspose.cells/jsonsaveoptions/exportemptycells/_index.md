---
title: "JsonSaveOptions.ExportEmptyCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Indica si se exportan celdas vacías como null"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/exportemptycells/
---
## JsonSaveOptions.ExportEmptyCells property

Indica si se exportan celdas vacías como null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar datos con algunas celdas vacías
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue(2.99); // B2 is intentionally left empty

            // Crear JsonSaveOptions con ExportEmptyCells establecido en false
            JsonSaveOptions options = new JsonSaveOptions
            {
                ExportEmptyCells = false
            };

            // Guardar a JSON - las celdas vacías se omitirán
            workbook.Save("output_skip_empty.json", options);

            // Cambiar ExportEmptyCells a true
            options.ExportEmptyCells = true;

            // Guardar de nuevo - las celdas vacías se incluirán
            workbook.Save("output_include_empty.json", options);
        }
    }
}
```

### Ver también

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


