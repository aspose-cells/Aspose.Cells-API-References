---
title: "SqlScriptSaveOptions.HasHeaderRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Indica si el rango contiene fila de encabezado"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/
---
## SqlScriptSaveOptions.HasHeaderRow property

Indica si el rango contiene una fila de encabezado.

```csharp
public bool HasHeaderRow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar fila de encabezado y datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Bob");

            // Configurar opciones de exportación SQL con HasHeaderRow=true
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                HasHeaderRow = true,
                CreateTable = true
            };

            // Guardar como script SQL
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script with header row exported successfully.");
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


