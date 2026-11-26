---
title: "SqlScriptSaveOptions.CheckAllDataForColumnType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Verifica todos los datos para encontrar el tipo de datos de las columnas"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/
---
## SqlScriptSaveOptions.CheckAllDataForColumnType property

Comprobar todos los datos para encontrar el tipo de datos de las columnas.

```csharp
public bool CheckAllDataForColumnType { get; set; }
```

### Observaciones

El valor predeterminado es false, solo verificamos la primera fila por rendimiento. Si esta propiedad es true y las columnas contienen tipos de valor mixtos, el tipo de las columnas será texto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckAllDataForColumnTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de muestra con tipos mixtos
            sheet.Cells["A1"].PutValue("First_name");
            sheet.Cells["B1"].PutValue("Last_name");
            sheet.Cells["C1"].PutValue("age");
            sheet.Cells["D1"].PutValue("tax");
            
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue("Doe");
            sheet.Cells["C2"].PutValue(30);
            sheet.Cells["D2"].PutValue("10%");
            
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["B3"].PutValue("Smith");
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["D3"].PutValue(0.15);

            // Configurar opciones de guardado SQL
            SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
            sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
            sqlSaveOptions.CreateTable = true;
            sqlSaveOptions.CheckAllDataForColumnType = true; // This will examine all data to determine column types
            
            // Guardar como script SQL - el método Save no devuelve una cadena, por lo que necesitamos guardar primero y luego leer el archivo
            wb.Save("output.sql", sqlSaveOptions);
            
            // Leer el script SQL generado
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            
            Console.WriteLine("SQL Script generated:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


