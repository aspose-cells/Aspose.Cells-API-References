---
title: "SqlScriptSaveOptions.CreateTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Indica si se exporta el SQL de creación de tabla"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/createtable/
---
## SqlScriptSaveOptions.CreateTable property

Indica si se exporta sql al crear la tabla.

```csharp
public bool CreateTable { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCreateTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Configurar opciones de exportación SQL con CreateTable habilitado
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                CreateTable = true,
                TableName = "Employees",
                HasHeaderRow = true
            };

            // Guardar como script SQL
            workbook.Save("output.sql", options);
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


