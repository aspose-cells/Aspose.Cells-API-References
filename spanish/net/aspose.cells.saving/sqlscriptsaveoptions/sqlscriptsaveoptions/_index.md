---
title: "SqlScriptSaveOptions.SqlScriptSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor SqlScriptSaveOptions. Crea opciones para guardar un archivo sql"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions constructor

Crea opciones para guardar el archivo sql.

```csharp
public SqlScriptSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Crear SqlScriptSaveOptions usando el constructor
            SqlScriptSaveOptions options = new SqlScriptSaveOptions();
            options.OperatorType = SqlScriptOperatorType.Insert;
            options.AddBlankLineBetweenRows = true;

            // Guardar como script SQL
            workbook.Save("output.sql", options);
            
            // Mostrar el SQL generado
            Console.WriteLine("Generated SQL Script:");
            Console.WriteLine(System.IO.File.ReadAllText("output.sql"));
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


