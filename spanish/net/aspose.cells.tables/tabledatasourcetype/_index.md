---
title: "Enum TableDataSourceType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Tables.TableDataSourceType enum. Representa el tipo de origen de datos de la tabla"
type: docs
url: /es/net/aspose.cells.tables/tabledatasourcetype/
---
## TableDataSourceType enumeration

Representa el tipo de origen de datos de la tabla.

```csharp
public enum TableDataSourceType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Worksheet | `0` | Tabla de hoja de cálculo de Excel |
| SharePoint | `1` | Lista vinculada de SharePoint de lectura y escritura |
| XML | `2` | Tabla del mapeador XML |
| QueryTable | `3` | Tabla de consulta |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableDataSourceTypeDemo
    {
        public static void TableDataSourceTypeExample()
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

            // Agregar un ListObject (tabla) a la hoja de cálculo
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Establecer el nombre para mostrar de la tabla
            listObject.DisplayName = "SampleTable";

            // Establecer el tipo de origen de datos de la tabla
            TableDataSourceType dataSourceType = listObject.DataSourceType;

            // Salida del tipo de origen de datos
            Console.WriteLine("Data Source Type: " + dataSourceType);

            // Guarda el libro de trabajo
            workbook.Save("TableDataSourceTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


