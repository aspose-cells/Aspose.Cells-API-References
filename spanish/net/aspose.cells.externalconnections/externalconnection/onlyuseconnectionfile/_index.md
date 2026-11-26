---
title: "ExternalConnection.OnlyUseConnectionFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Indica si la aplicación de hoja de cálculo debe usar siempre y solo la información de conexión en el archivo de conexión externa indicado por el atributo odcFile cuando se actualiza la conexión. Si es false, la aplicación de hoja de cálculo debe seguir el procedimiento indicado por el atributo reconnectionMethod"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/
---
## ExternalConnection.OnlyUseConnectionFile property

Indica si la aplicación de hoja de cálculo debe siempre y solo usar la información de conexión en el archivo de conexión externa indicado por el atributo odcFile cuando se actualiza la conexión. Si false, entonces la aplicación de hoja de cálculo debe seguir el procedimiento indicado por el atributo reconnectionMethod.

```csharp
public bool OnlyUseConnectionFile { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOnlyUseConnectionFileDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor actual de OnlyUseConnectionFile
                Console.WriteLine("Initial OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Establecer un nuevo valor de OnlyUseConnectionFile (ya que es de lectura‑escritura)
                connection.OnlyUseConnectionFile = true;
                Console.WriteLine("Updated OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Alternar el valor para demostrar la capacidad de configuración
                connection.OnlyUseConnectionFile = !connection.OnlyUseConnectionFile;
                Console.WriteLine("Toggled OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("OnlyUseConnectionFileDemo.xlsx");
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


