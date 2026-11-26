---
title: "ExternalConnection.OdcFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Especifica la ruta completa al archivo de conexión externa desde el cual se creó esta conexión. Si una conexión falla durante un intento de actualizar datos y reconnectionMethod1, la aplicación de hoja de cálculo volverá a intentarlo usando la información del archivo de conexión externa en lugar del objeto de conexión incrustado en el libro."
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/odcfile/
---
## ExternalConnection.OdcFile property

Especifica la ruta completa al archivo de conexión externa desde el cual se creó esta conexión. Si una conexión falla durante un intento de actualizar datos, y reconnectionMethod=1, entonces la aplicación de hoja de cálculo volverá a intentarlo usando la información del archivo de conexión externa en lugar del objeto de conexión incrustado en el libro.

```csharp
public string OdcFile { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOdcFileDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Muestre el valor actual de OdcFile
                Console.WriteLine("Initial OdcFile value: " + connection.OdcFile);
                
                // Establezca un nuevo valor de OdcFile (ya que es de lectura-escritura)
                connection.OdcFile = @"C:\Connections\ExternalData.odc";
                Console.WriteLine("Updated OdcFile value: " + connection.OdcFile);
                
                // Borre el valor de OdcFile
                connection.OdcFile = string.Empty;
                Console.WriteLine("Cleared OdcFile value: " + connection.OdcFile);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("OdcFileDemo.xlsx");
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


