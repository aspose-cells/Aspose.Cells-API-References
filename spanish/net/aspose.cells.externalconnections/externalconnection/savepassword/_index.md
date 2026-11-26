---
title: "ExternalConnection.SavePassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ExternalConnection property. Verdadero si la contraseña debe guardarse como parte de la cadena de conexión, de lo contrario Falso"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/savepassword/
---
## ExternalConnection.SavePassword property

True si la contraseña debe guardarse como parte de la cadena de conexión; de lo contrario, False.

```csharp
public bool SavePassword { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySavePasswordDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];

                // Mostrar el valor actual de SavePassword
                Console.WriteLine("Initial SavePassword value: " + connection.SavePassword);

                // Demuestre la configuración de la propiedad (ya que es de lectura-escritura)
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Updated SavePassword value: " + connection.SavePassword);

                // Alternar el valor para demostrar la capacidad de configuración
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Toggled SavePassword value: " + connection.SavePassword);

                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("SavePasswordDemo.xlsx");
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


