---
title: "ExternalConnection.BackgroundRefresh"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Indica si la conexión puede actualizarse en segundo plano de forma asíncrona. true si el uso preferido de la conexión es actualizar de forma asíncrona en segundo plano, false si el uso preferido es actualizar de forma síncrona en primer plano."
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/backgroundrefresh/
---
## ExternalConnection.BackgroundRefresh property

Indica si la conexión puede actualizarse en segundo plano (asíncronamente). true si el uso preferido de la conexión es actualizar asíncronamente en segundo plano; false si el uso preferido de la conexión es actualizar sincrónicamente en primer plano.

```csharp
public bool BackgroundRefresh { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyBackgroundRefreshDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Muestre el valor actual de BackgroundRefresh
                Console.WriteLine("Initial BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Cambie el valor de BackgroundRefresh
                connection.BackgroundRefresh = !connection.BackgroundRefresh;
                Console.WriteLine("Updated BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("BackgroundRefreshDemo.xlsx");
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


