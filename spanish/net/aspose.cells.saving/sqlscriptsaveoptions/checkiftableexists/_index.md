---
title: "SqlScriptSaveOptions.CheckIfTableExists"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "SqlScriptSaveOptions property. Verifica si el nombre de la tabla existe antes de crear"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/
---
## SqlScriptSaveOptions.CheckIfTableExists property

Comprobar si el nombre de la tabla existe antes de crearla

```csharp
public bool CheckIfTableExists { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckIfTableExistsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Configurar opciones de guardado SQL
            SqlScriptSaveOptions sqlOptions = new SqlScriptSaveOptions();
            sqlOptions.CreateTable = true;
            sqlOptions.CheckIfTableExists = true;
            sqlOptions.OperatorType = SqlScriptOperatorType.Insert;

            // Guardar en archivo de script SQL
            workbook.Save("output.sql", sqlOptions);

            // Leer y mostrar el SQL generado
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            Console.WriteLine("Generated SQL Script:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


