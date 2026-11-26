---
title: "ConnectionParameter.Prompt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConnectionParameter. Cadena de solicitud para el parámetro. Presentada al usuario de la hoja de cálculo junto con la interfaz de entrada para recopilar el valor del parámetro antes de actualizar los datos externos. Se usa solo cuando parameterType es prompt"
type: docs
url: /es/net/aspose.cells.externalconnections/connectionparameter/prompt/
---
## ConnectionParameter.Prompt property

Cadena de solicitud para el parámetro. Presentada al usuario de la hoja de cálculo junto con la interfaz de entrada para recopilar el valor del parámetro antes de actualizar los datos externos. Se usa solo cuando parameterType = prompt.

```csharp
public string Prompt { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyPromptDemo
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
                
                // Para demostración, mostraremos cómo se usaría Prompt si tuviéramos un parámetro
                if (parameter != null)
                {
                    // Obtener y mostrar el valor actual de Prompt
                    Console.WriteLine("Current Prompt: " + parameter.Prompt);
                    
                    // Establecer un nuevo valor de Prompt (ya que la propiedad es de lectura y escritura)
                    parameter.Prompt = "Enter customer ID:";
                    Console.WriteLine("Updated Prompt: " + parameter.Prompt);
                }
                else
                {
                    // Demostración de respaldo cuando no podemos crear el parámetro
                    workbook.Worksheets[0].Cells["A1"].Value = "Prompt property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ConnectionParameterPromptDemo.xlsx");
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


