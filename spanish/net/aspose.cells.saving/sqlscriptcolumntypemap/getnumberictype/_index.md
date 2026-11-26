---
title: "SqlScriptColumnTypeMap.GetNumbericType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SqlScriptColumnTypeMap. Obtiene el tipo numérico en la base de datos"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/
---
## SqlScriptColumnTypeMap.GetNumbericType method

Obtiene el tipo numérico en la base de datos.

```csharp
[Obsolete("Use SqlScriptColumnTypeMap.GetNumberType() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetNumbericType()
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método SqlScriptColumnTypeMap.GetNumberType(). Este método será eliminado 6 meses después a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetNumbericTypeDemo
    {
        public static void Run()
        {
            // Crea una instancia de SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Obtener y mostrar el mapeo de tipos numéricos
            string numericType = columnTypeMap.GetNumbericType();
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Crear un libro de trabajo simple con datos numéricos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue(123.45);

            // Guardar con opciones de script SQL usando el mapeo de tipos
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            workbook.Save("NumericTypeDemo.sql", saveOptions);
        }
    }
}
```

### Ver también

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


