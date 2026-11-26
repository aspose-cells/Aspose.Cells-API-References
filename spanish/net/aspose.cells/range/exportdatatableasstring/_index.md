---
title: "Range.ExportDataTableAsString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Exporta los datos de este rango a un objeto DataTable"
type: docs
url: /es/net/aspose.cells/range/exportdatatableasstring/
---
## Range.ExportDataTableAsString method

Exporta los datos de este rango a un objeto DataTable.

```csharp
public DataTable ExportDataTableAsString()
```

### Valor de retorno

Objeto DataTable exportado.

### Observaciones

Todos los datos en la colección [`Cells`](../../cells/) se convierten a cadenas.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableAsStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(30);

            // Obtener el rango que contiene datos
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            try
            {
                // Llamar al método ExportDataTableAsString
                DataTable dataTable = range.ExportDataTableAsString();

                // Mostrar los datos exportados
                Console.WriteLine("Exported DataTable:");
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}, {row[1]}");
                }

                // Guarda el libro de trabajo
                workbook.Save("RangeMethodExportDataTableAsStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportDataTableAsString method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


