---
title: "JsonSaveOptions.ExportArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Obtiene o establece el rango de exportación"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/exportarea/
---
## JsonSaveOptions.ExportArea property

Obtiene o establece el rango de exportación.

```csharp
public CellArea ExportArea { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Configurar opciones de guardado JSON con ExportArea
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Guardar con el área de exportación especificada (A1:B3)
            workbook.Save("JsonExportAreaDemo.json", saveOptions);
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


