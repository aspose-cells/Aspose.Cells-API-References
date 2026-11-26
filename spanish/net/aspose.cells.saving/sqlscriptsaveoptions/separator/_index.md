---
title: "SqlScriptSaveOptions.Separator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Obtiene y establece el separador de caracteres del script sql"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/separator/
---
## SqlScriptSaveOptions.Separator property

Obtiene y establece el separador de caracteres del script sql.

```csharp
public char Separator { get; set; }
```

### Observaciones

Solo puede ser ' ' o '\\n'. Si el

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("John");

            // Configurar opciones de guardado SQL con separador personalizado
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                Separator = ';',
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Guarda con separador personalizado
            workbook.Save("SqlScriptWithSeparator.sql", saveOptions);

            Console.WriteLine("SQL script saved with custom separator.");
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


