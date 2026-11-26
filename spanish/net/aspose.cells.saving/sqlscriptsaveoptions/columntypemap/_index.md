---
title: "SqlScriptSaveOptions.ColumnTypeMap"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Obtiene y establece el mapa de tipos de columna para diferentes bases de datos"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/columntypemap/
---
## SqlScriptSaveOptions.ColumnTypeMap property

Obtiene y establece el mapa de tipos de columna para diferentes bases de datos.

```csharp
public SqlScriptColumnTypeMap ColumnTypeMap { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyColumnTypeMapDemo
    {
        public static void Run()
        {
            // Crear un mapa de tipos de columna personalizado
            SqlScriptColumnTypeMap customTypeMap = new SqlScriptColumnTypeMap();
            
            // Crear opciones de guardado SQL
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                ColumnTypeMap = customTypeMap,
                CheckIfTableExists = true,
                ExportAsString = false
            };

            // Crear libro de trabajo de ejemplo con datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar encabezados
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Salary");
            
            // Agregar filas de datos
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Smith");
            worksheet.Cells["C2"].PutValue(5000.50);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane Doe");
            worksheet.Cells["C3"].PutValue(6500.75);

            // Guardar como script SQL
            workbook.Save("EmployeeData.sql", saveOptions);
            
            Console.WriteLine("SQL script generated successfully with custom column type mapping.");
        }
    }
}
```

### Ver también

* class [SqlScriptColumnTypeMap](../../sqlscriptcolumntypemap/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


