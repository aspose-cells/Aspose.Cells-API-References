---
title: "Clase SqlScriptColumnTypeMap"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Saving.SqlScriptColumnTypeMap. Representa el mapa de tipos de columna"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptcolumntypemap/
---
## SqlScriptColumnTypeMap class

Representa el mapa de tipos de columna.

```csharp
public class SqlScriptColumnTypeMap
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SqlScriptColumnTypeMap](sqlscriptcolumntypemap/)() | El constructor predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [GetNumbericType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/)() | (**Obsolete.**) Obtiene el tipo numérico en la base de datos. |
| virtual [GetNumberType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumbertype/)() | Obtiene el tipo numérico en la base de datos. |
| virtual [GetStringType](../../aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/)() | Obtiene el tipo de cadena en la base de datos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptColumnTypeMapDemo
    {
        public static void SqlScriptColumnTypeMapExample()
        {
            // Crea una instancia de SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Demuestra el uso de los métodos GetStringType y GetNumbericType
            string stringType = columnTypeMap.GetStringType();
            string numericType = columnTypeMap.GetNumbericType();

            // Muestra los resultados en la consola
            Console.WriteLine("String Type in Database: " + stringType);
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Crea una instancia de SqlScriptSaveOptions y establece el ColumnTypeMap
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };

            // Crea un libro de trabajo y agrega algunos datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Guarda el libro de trabajo como script SQL usando las opciones de guardado
            workbook.Save("SqlScriptExample.sql", saveOptions);

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


