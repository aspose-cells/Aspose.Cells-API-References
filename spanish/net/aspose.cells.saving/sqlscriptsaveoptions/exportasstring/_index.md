---
title: "SqlScriptSaveOptions.ExportAsString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Indica si se exportan todos los datos como valor de cadena"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/exportasstring/
---
## SqlScriptSaveOptions.ExportAsString property

Indica si se exportan todos los datos como valor de cadena.

```csharp
public bool ExportAsString { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyExportAsStringDemo
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

            // Configurar opciones de exportación SQL
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                ExportAsString = true, // Demonstrating ExportAsString property
                HasHeaderRow = true
            };

            // Guardar con exportación de cadena habilitada
            workbook.Save("ExportAsString_True.sql", saveOptions);

            // Cambie a false y guarde nuevamente
            saveOptions.ExportAsString = false;
            workbook.Save("ExportAsString_False.sql", saveOptions);

            Console.WriteLine("SQL scripts saved with different ExportAsString settings.");
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


