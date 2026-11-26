---
title: "ExternalConnection.KeepAlive"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Verdadero cuando la aplicación de hoja de cálculo debe hacer esfuerzos para mantener la conexión abierta. Cuando es falso, la aplicación debe cerrar la conexión después de recuperar la información."
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/keepalive/
---
## ExternalConnection.KeepAlive property

True cuando la aplicación de hoja de cálculo debe esforzarse por mantener la conexión abierta. Cuando false, la aplicación debe cerrar la conexión después de recuperar la información.

```csharp
public bool KeepAlive { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyKeepAliveDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor actual de KeepAlive
                Console.WriteLine("Initial KeepAlive value: " + connection.KeepAlive);
                
                // Alternar el valor de KeepAlive ya que es de lectura-escritura
                connection.KeepAlive = !connection.KeepAlive;
                Console.WriteLine("Updated KeepAlive value: " + connection.KeepAlive);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("KeepAliveDemo.xlsx");
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


