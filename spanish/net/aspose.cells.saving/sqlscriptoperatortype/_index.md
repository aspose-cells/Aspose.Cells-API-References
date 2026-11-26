---
title: "Enum SqlScriptOperatorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Saving.SqlScriptOperatorType enum. Representa el tipo de datos operativos"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptoperatortype/
---
## SqlScriptOperatorType enumeration

Representa el tipo de datos operativos.

```csharp
public enum SqlScriptOperatorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Insert | `0` | Insertar datos. |
| Update | `1` | Actualizar datos. |
| Delete | `2` | Eliminar datos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptOperatorTypeDemo
    {
        public static void SqlScriptOperatorTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Crear SqlScriptSaveOptions y establecer propiedades.
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                AddBlankLineBetweenRows = true,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "SampleTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Guardar el libro de trabajo como script SQL.
            workbook.Save("SqlScriptOperatorTypeExample.sql", saveOptions);

            // Genere la salida de los resultados
            Console.WriteLine("SQL script has been saved successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


