---
title: "QueryTable.ResultRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad QueryTable. Obtiene el rango del resultado"
type: docs
url: /es/net/aspose.cells/querytable/resultrange/
---
## QueryTable.ResultRange property

Obtiene el rango del resultado.

```csharp
public Range ResultRange { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyResultRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para simular una tabla de consulta
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Verifique si hay tablas de consulta en la hoja de cálculo
                if (worksheet.QueryTables.Count > 0)
                {
                    // Obtenga la primera tabla de consulta
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Mostrar el valor de la propiedad ResultRange (operación de solo lectura)
                    Aspose.Cells.Range resultRange = queryTable.ResultRange;
                    Console.WriteLine("ResultRange Address: " + resultRange.Address);
                    Console.WriteLine("ResultRange Row Count: " + resultRange.RowCount);
                    Console.WriteLine("ResultRange Column Count: " + resultRange.ColumnCount);
                    Console.WriteLine("ResultRange First Row: " + resultRange.FirstRow);
                    Console.WriteLine("ResultRange First Column: " + resultRange.FirstColumn);

                    // Mostrar los valores en el rango de resultados
                    Console.WriteLine("Values in ResultRange:");
                    foreach (Cell cell in resultRange)
                    {
                        Console.WriteLine($"Cell [{cell.Row}, {cell.Column}]: {cell.Value}");
                    }
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Guarda el libro de trabajo
                workbook.Save("ResultRangeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


