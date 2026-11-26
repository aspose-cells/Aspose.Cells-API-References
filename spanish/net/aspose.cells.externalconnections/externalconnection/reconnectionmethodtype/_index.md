---
title: "ExternalConnection.ReconnectionMethodType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/
---
## ExternalConnection.ReconnectionMethodType property

Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla. El valor predeterminado es ReConnectionMethodType.Required.

```csharp
public ReConnectionMethodType ReconnectionMethodType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyReconnectionMethodTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor actual de ReconnectionMethodType
                Console.WriteLine("Initial ReconnectionMethodType: " + connection.ReconnectionMethodType);
                
                // Demuestre la configuración de la propiedad (ya que es de lectura-escritura)
                connection.ReconnectionMethodType = ReConnectionMethodType.Always;
                Console.WriteLine("Updated ReconnectionMethodType: " + connection.ReconnectionMethodType);
                
                // Recorrer los valores posibles para demostrar la capacidad de configuración
                foreach (ReConnectionMethodType method in Enum.GetValues(typeof(ReConnectionMethodType)))
                {
                    connection.ReconnectionMethodType = method;
                    Console.WriteLine($"ReconnectionMethodType set to: {method}");
                }
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("ReconnectionMethodTypeDemo.xlsx");
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

* enum [ReConnectionMethodType](../../reconnectionmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


