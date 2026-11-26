---
title: "SqlScriptSaveOptions.PrimaryKey"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Representa qué columna es la clave primaria de la tabla de datos"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/primarykey/
---
## SqlScriptSaveOptions.PrimaryKey property

Representa qué columna es la clave primaria de la tabla de datos.

```csharp
public int PrimaryKey { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyPrimaryKeyDemo
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

            // Configurar opciones de exportación SQL con PrimaryKey establecido en la primera columna (0)
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                PrimaryKey = 0,
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Guardar como script SQL
            workbook.Save("EmployeesExport.sql", saveOptions);

            Console.WriteLine("SQL script exported with PrimaryKey set to column 0 (ID)");
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


