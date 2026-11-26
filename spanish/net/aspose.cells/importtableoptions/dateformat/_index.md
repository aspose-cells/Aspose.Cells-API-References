---
title: "ImportTableOptions.DateFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ImportTableOptions property. Obtiene o establece la cadena de formato de fecha para celdas con valores de fecha y hora importados"
type: docs
url: /es/net/aspose.cells/importtableoptions/dateformat/
---
## ImportTableOptions.DateFormat property

Obtiene o establece la cadena de formato de fecha para celdas con valores de fecha y hora importados.

```csharp
public string DateFormat { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una DataTable de ejemplo con valores de fecha
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("DateColumn", typeof(DateTime));
            dataTable.Rows.Add(new DateTime(2023, 1, 15));
            dataTable.Rows.Add(new DateTime(2023, 2, 20));
            dataTable.Rows.Add(new DateTime(2023, 3, 25));

            // Definir el rango de importación
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 10, 1);

            // Importar datos con formato de fecha personalizado
            worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions()
            {
                IsFieldNameShown = true,
                DateFormat = "YYYY-MM-DD"
            });

            // Guardar el libro de trabajo para demostrar el resultado
            workbook.Save("DateFormatDemoOutput.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


