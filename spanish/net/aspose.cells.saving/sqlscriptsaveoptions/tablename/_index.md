---
title: "SqlScriptSaveOptions.TableName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Obtiene y establece el nombre de la tabla"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/tablename/
---
## SqlScriptSaveOptions.TableName property

Obtiene y establece el nombre de la tabla.

```csharp
public string TableName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyTableNameDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con algunos datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Configura las opciones de guardado SQL con un nombre de tabla personalizado
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions();
            saveOptions.TableName = "Employees"; // Demonstrating TableName property
            saveOptions.CreateTable = true;
            saveOptions.OperatorType = SqlScriptOperatorType.Insert;

            // Guardar como script SQL
            workbook.Save("output.sql", saveOptions);

            Console.WriteLine("SQL Script generated with table name 'Employees'");
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


