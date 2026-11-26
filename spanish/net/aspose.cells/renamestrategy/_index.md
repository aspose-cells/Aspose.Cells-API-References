---
title: "Enumeración RenameStrategy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.RenameStrategy. Opción de estrategia para nombres duplicados de columnas"
type: docs
url: /es/net/aspose.cells/renamestrategy/
---
## RenameStrategy enumeration

Opción de estrategia para nombres duplicados de columnas.

```csharp
public enum RenameStrategy
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Exception | `0` | Lanza una excepción. |
| Digit | `1` | Nombrado con dígito. Los nombres duplicados se convertirán en ...1, ...2, etc. |
| Letter | `2` | Nombrado con letra.. Los nombres duplicados se convertirán en ...A, ...B, etc. |

### Observaciones

Al procesar datos con encabezados, algunos escenarios requieren que los encabezados no se dupliquen en ninguna columna. Por ejemplo, al exportar datos a una DataTable y que el encabezado deba tomarse como el nombre de columna de la DataTable, los valores duplicados del encabezado son inválidos. Para este tipo de situaciones, el usuario puede determinar cómo manejarlos especificando esta estrategia.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RenameStrategyDemo
    {
        public static void RenameStrategyExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("John");

            // Cree ExportTableOptions y establezca el RenameStrategy
            ExportTableOptions options = new ExportTableOptions
            {
                RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
            };

            // Exporte los datos de la hoja de cálculo a una DataTable
            System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);

            // Muestre el contenido de la DataTable
            foreach (System.Data.DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Guarda el libro de trabajo
            workbook.Save("RenameStrategyExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


