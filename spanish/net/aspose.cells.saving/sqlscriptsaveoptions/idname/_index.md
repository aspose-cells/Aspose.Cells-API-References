---
title: "SqlScriptSaveOptions.IdName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Obtiene y establece el nombre de la columna id"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/idname/
---
## SqlScriptSaveOptions.IdName property

Obtiene y establece el nombre de la columna id.

```csharp
public string IdName { get; set; }
```

### Observaciones

Si esta propiedad está establecida, se insertará una columna con un valor entero de incremento automático.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyIdNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // Configurar opciones de exportación SQL con IdName
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Guardar como script SQL
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script exported with IdName property");
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


