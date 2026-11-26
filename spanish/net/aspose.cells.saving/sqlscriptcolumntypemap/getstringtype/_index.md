---
title: "SqlScriptColumnTypeMap.GetStringType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "SqlScriptColumnTypeMap método. Obtiene el tipo de cadena en la base de datos"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/
---
## SqlScriptColumnTypeMap.GetStringType method

Obtiene el tipo de cadena en la base de datos.

```csharp
public virtual string GetStringType()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetStringTypeDemo
    {
        public static void Run()
        {
            // Crea una instancia de SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Obtener y mostrar el tipo de cadena predeterminado
            string stringType = columnTypeMap.GetStringType();
            Console.WriteLine("Default String Type: " + stringType);

            // Crear un libro de trabajo simple con datos de cadena
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John Doe");

            // Guardar con opciones de script SQL usando el mapa de tipos
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            
            workbook.Save("SqlScriptOutput.sql", saveOptions);
            Console.WriteLine("SQL script saved with string type: " + stringType);
        }
    }
}
```

### Ver también

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


