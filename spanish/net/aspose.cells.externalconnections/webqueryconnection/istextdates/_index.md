---
title: "WebQueryConnection.IsTextDates"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de WebQueryConnection. Bandera que indica si las fechas deben importarse en las celdas de la hoja de cálculo como texto en lugar de como fechas."
type: docs
url: /es/net/aspose.cells.externalconnections/webqueryconnection/istextdates/
---
## WebQueryConnection.IsTextDates property

Indicador que indica si las fechas deben importarse a las celdas de la hoja de cálculo como texto en lugar de como fechas.

```csharp
public bool IsTextDates { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsTextDatesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceder a la primera hoja de cálculo
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Cree una conexión de consulta web cargándola desde un archivo existente.
                // o accediendo a una conexión existente.
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Muestre el valor inicial de IsTextDates.
                    Console.WriteLine("Initial IsTextDates value: " + connection.IsTextDates);
                    
                    // Establezca IsTextDates en true.
                    connection.IsTextDates = true;
                    Console.WriteLine("Updated IsTextDates value: " + connection.IsTextDates);
                    
                    // Restablezca IsTextDates a false.
                    connection.IsTextDates = false;
                    Console.WriteLine("Final IsTextDates value: " + connection.IsTextDates);
                    
                    // Guardar el libro con la conexión de consulta web
                    workbook.Save("WebQueryConnectionIsTextDatesDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


