---
title: "Enum ConnectionParameterType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ExternalConnections.ConnectionParameterType enum. Especifica el tipo de parámetro de la conexión externa"
type: docs
url: /es/net/aspose.cells.externalconnections/connectionparametertype/
---
## ConnectionParameterType enumeration

Especifica el tipo de parámetro de la conexión externa

```csharp
public enum ConnectionParameterType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Cell | `0` | Obtenga el valor del parámetro de una celda en cada actualización. |
| Prompt | `1` | Solicite al usuario en cada actualización un valor de parámetro. |
| Value | `2` | Utilice un valor constante en cada actualización para el valor del parámetro. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Demostrar la creación y uso de valores del enum ConnectionParameterType
                ConnectionParameterType cellParam = ConnectionParameterType.Cell;
                ConnectionParameterType promptParam = ConnectionParameterType.Prompt;
                ConnectionParameterType valueParam = ConnectionParameterType.Value;

                // Mostrar los valores del enum
                Console.WriteLine("Connection Parameter Types:");
                Console.WriteLine($"Cell: {cellParam}");
                Console.WriteLine($"Prompt: {promptParam}");
                Console.WriteLine($"Value: {valueParam}");

                // Demostrar uso en una sentencia switch
                ConnectionParameterType testParam = ConnectionParameterType.Prompt;
                switch (testParam)
                {
                    case ConnectionParameterType.Cell:
                        Console.WriteLine("Parameter will get value from a cell");
                        break;
                    case ConnectionParameterType.Prompt:
                        Console.WriteLine("Parameter will prompt user for value");
                        break;
                    case ConnectionParameterType.Value:
                        Console.WriteLine("Parameter will use constant value");
                        break;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating ConnectionParameterType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


