---
title: "ExternalConnection.RefreshOnLoad"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. True si esta conexión debe actualizarse al abrir el archivo, de lo contrario false"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/refreshonload/
---
## ExternalConnection.RefreshOnLoad property

True si esta conexión debe actualizarse al abrir el archivo; de lo contrario, false.

```csharp
public bool RefreshOnLoad { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshOnLoadDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceder a la primera conexión externa (el libro de trabajo viene con conexiones predeterminadas)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor inicial de RefreshOnLoad
                Console.WriteLine("Initial RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Demuestre la configuración de la propiedad (ya que es de lectura-escritura)
                connection.RefreshOnLoad = !connection.RefreshOnLoad;
                Console.WriteLine("Updated RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("RefreshOnLoadDemo.xlsx");
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


