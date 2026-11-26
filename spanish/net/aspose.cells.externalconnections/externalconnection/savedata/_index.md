---
title: "ExternalConnection.SaveData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalConnection. Verdadero si los datos externos obtenidos a través de la conexión para rellenar una tabla deben guardarse con el libro de trabajo, de lo contrario falso"
type: docs
url: /es/net/aspose.cells.externalconnections/externalconnection/savedata/
---
## ExternalConnection.SaveData property

True si los datos externos obtenidos a través de la conexión para rellenar una tabla deben guardarse con el libro; de lo contrario, false.

```csharp
public bool SaveData { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySaveDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceda a la primera conexión externa (suponiendo que exista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mostrar el valor actual de SaveData
                Console.WriteLine("Initial SaveData value: " + connection.SaveData);
                
                // Demuestre la configuración de la propiedad (ya que es de lectura-escritura)
                connection.SaveData = !connection.SaveData;
                Console.WriteLine("Updated SaveData value: " + connection.SaveData);
                
                // Guarde el libro con la configuración de conexión modificada
                workbook.Save("SaveDataDemo.xlsx");
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


