---
title: "ExternalConnection.SecondCommand"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ExternalConnection property. Especifica una cadena de texto de segundo comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command, sin cláusula WHERE presente en este último. Con base en estos 2 comandos, commandsCommand y ServerCommand, la UI de parámetros puede poblarse y pueden construirse consultas parametrizadas."
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/secondcommand/
---
## ExternalConnection.SecondCommand property

Especifica una segunda cadena de texto de comando que se conserva cuando se utilizan campos de página basados en servidor de PivotTable. Para conexiones ODBC, serverCommand suele ser una consulta más amplia que command (no hay cláusula WHERE presente en la primera). Basado en estos 2 comandos (Command y ServerCommand), la interfaz de usuario de parámetros puede poblarse y pueden construirse consultas parametrizadas

```csharp
public virtual string SecondCommand { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor actual de SecondCommand (operación de lectura)
                Console.WriteLine("Initial SecondCommand value: " + connection.SecondCommand);
                
                // Establecer un nuevo valor de SecondCommand (ya que es de lectura-escritura)
                connection.SecondCommand = "SELECT * FROM Customers WHERE Country = 'USA'";
                Console.WriteLine("Updated SecondCommand value: " + connection.SecondCommand);
                
                // Borrar el SecondCommand para demostrar la configuración de una cadena vacía
                connection.SecondCommand = string.Empty;
                Console.WriteLine("Cleared SecondCommand value: " + connection.SecondCommand);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("SecondCommandDemo.xlsx");
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


