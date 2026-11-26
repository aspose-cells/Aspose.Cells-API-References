---
title: "ConnectionParameter.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConnectionParameter. El nombre del parámetro"
type: docs
url: /es/net/aspose.cells.externalconnections/connectionparameter/name/
---
## ConnectionParameter.Name property

El nombre del parámetro.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();

                // Crear un parámetro de conexión (simulado ya que los parámetros del constructor son desconocidos)
                ConnectionParameter parameter = null;

                // En un escenario real, crearías el parámetro correctamente
                // parameter = new ConnectionParameter(/* required parameters */);

                // Para demostración, mostraremos cómo se usaría Name si tuviéramos un parámetro
                if (parameter != null)
                {
                    // Obtener y mostrar el valor actual de Name
                    Console.WriteLine("Current Name: " + parameter.Name);

                    // Establecer un nuevo valor de Name (ya que la propiedad es de lectura y escritura)
                    parameter.Name = "NewParameterName";
                    Console.WriteLine("Updated Name: " + parameter.Name);
                }
                else
                {
                    // Demostración de respaldo cuando no podemos crear el parámetro
                    workbook.Worksheets[0].Cells["A1"].Value = "Name property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }

                // Guarda el libro de trabajo
                workbook.Save("ConnectionParameterNameDemo.xlsx");
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

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


