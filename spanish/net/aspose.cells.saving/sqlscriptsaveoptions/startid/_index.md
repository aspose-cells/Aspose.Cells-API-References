---
title: "SqlScriptSaveOptions.StartId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Obtiene y establece el id inicial"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/startid/
---
## SqlScriptSaveOptions.StartId property

Obtiene y establece el id inicial.

```csharp
public int StartId { get; set; }
```

### Observaciones

Solo funciona cuando [`IdName`](../idname/) está configurado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyStartIdDemo
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

            // Configurar opciones de exportación SQL con StartId establecido en 100
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                StartId = 100, // Demonstrating StartId property
                HasHeaderRow = true,
                OperatorType = SqlScriptOperatorType.Insert
            };

            // Guardar como script SQL
            workbook.Save("Employees_WithStartId.sql", saveOptions);
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


