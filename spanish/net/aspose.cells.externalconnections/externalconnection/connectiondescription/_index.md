---
title: "ExternalConnection.ConnectionDescription"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Especifica la descripción del usuario para esta conexión"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/connectiondescription/
---
## ExternalConnection.ConnectionDescription property

Especifica la descripción del usuario para esta conexión

```csharp
public string ConnectionDescription { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyConnectionDescriptionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Agregar una hoja de cálculo con datos de ejemplo
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Sales";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1000;
                worksheet.Cells["A3"].Value = "Banana";
                worksheet.Cells["B3"].Value = 2000;

                // Crear una tabla dinámica para establecer una conexión externa
                int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Obtenga la conexión externa de la tabla dinámica
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // Mostrar el valor inicial de ConnectionDescription
                Console.WriteLine("Initial ConnectionDescription: " + connection.ConnectionDescription);

                // Establecer una nueva descripción (ya que es de lectura-escritura)
                connection.ConnectionDescription = "This connection retrieves sales data from internal sources";
                Console.WriteLine("Updated ConnectionDescription: " + connection.ConnectionDescription);

                // Borrar la descripción
                connection.ConnectionDescription = string.Empty;
                Console.WriteLine("Cleared ConnectionDescription: " + connection.ConnectionDescription);

                // Guardar el libro de trabajo con la conexión modificada
                workbook.Save("ConnectionDescriptionDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


