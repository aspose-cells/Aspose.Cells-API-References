---
title: "ExternalConnection.IsNew"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Verdadero si la conexión no se ha actualizado por primera vez, de lo contrario falso. Este estado puede ocurrir cuando el usuario guarda el archivo antes de que una consulta haya terminado de devolver resultados"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/isnew/
---
## ExternalConnection.IsNew property

True si la conexión no se ha actualizado por primera vez; de lo contrario, false. Este estado puede ocurrir cuando el usuario guarda el archivo antes de que una consulta haya terminado de devolver resultados.

```csharp
public bool IsNew { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsNewDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceder a la primera conexión externa (las conexiones recién creadas suelen ser "IsNew")
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor inicial de IsNew
                Console.WriteLine("Initial IsNew value: " + connection.IsNew);
                
                // Dado que IsNew es de lectura-escritura, demostrar cómo establecerlo
                connection.IsNew = false;
                Console.WriteLine("Updated IsNew value: " + connection.IsNew);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("IsNewDemo.xlsx");
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


