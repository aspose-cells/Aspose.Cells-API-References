---
title: "SqlScriptSaveOptions.OperatorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Obtiene y establece el tipo de operador de sql"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/operatortype/
---
## SqlScriptSaveOptions.OperatorType property

Obtiene y establece el tipo de operador de sql.

```csharp
public SqlScriptOperatorType OperatorType { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyOperatorTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Id");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Configurar opciones de guardado SQL
            SqlScriptSaveOptions options = new SqlScriptSaveOptions();
            options.OperatorType = SqlScriptOperatorType.Delete;
            options.IdName = "Id";
            options.Separator = '\n';
            options.AddBlankLineBetweenRows = true;
            options.CreateTable = true;

            // Guardar en un flujo de memoria y obtener el script SQL como cadena
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string sqlScript = reader.ReadToEnd();
                    
                    // Mostrar el SQL generado
                    Console.WriteLine("Generated SQL Script:");
                    Console.WriteLine(sqlScript);
                }
            }
        }
    }
}
```

### Ver también

* enum [SqlScriptOperatorType](../../sqlscriptoperatortype/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


