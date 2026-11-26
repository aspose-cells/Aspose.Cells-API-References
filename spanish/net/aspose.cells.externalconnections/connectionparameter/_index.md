---
title: "Clase ConnectionParameter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ExternalConnections.ConnectionParameter. Especifica propiedades de cualquier parámetro utilizado con conexiones de datos externas. Los parámetros son válidos para ODBC y consultas web."
type: docs
url: /es/net/aspose.cells.externalconnections/connectionparameter/
---
## ConnectionParameter class

Especifica propiedades sobre cualquier parámetro usado con conexiones de datos externas. Los parámetros son válidos para ODBC y consultas web.

```csharp
public class ConnectionParameter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CellReference](../../aspose.cells.externalconnections/connectionparameter/cellreference/) { get; set; } | Referencia de celda que indica el valor de cuál celda usar para el parámetro de consulta. Se usa solo cuando parameterType es cell. |
| [Name](../../aspose.cells.externalconnections/connectionparameter/name/) { get; set; } | El nombre del parámetro. |
| [Prompt](../../aspose.cells.externalconnections/connectionparameter/prompt/) { get; set; } | Cadena de solicitud para el parámetro. Presentada al usuario de la hoja de cálculo junto con la interfaz de entrada para recopilar el valor del parámetro antes de actualizar los datos externos. Se usa solo cuando parameterType = prompt. |
| [RefreshOnChange](../../aspose.cells.externalconnections/connectionparameter/refreshonchange/) { get; set; } | Indicador que indica si la consulta debe actualizarse automáticamente cuando el contenido de una celda que proporciona el valor del parámetro cambia. Si true, los datos externos se actualizan usando el nuevo valor del parámetro cada vez que hay un cambio. Si false, los datos externos solo se actualizan cuando lo solicita el usuario, o cuando otro evento desencadena la actualización (p. ej., al abrir el libro de trabajo). |
| [SqlType](../../aspose.cells.externalconnections/connectionparameter/sqltype/) { get; set; } | Tipo de datos SQL del parámetro. Válido solo para fuentes ODBC. |
| [Type](../../aspose.cells.externalconnections/connectionparameter/type/) { get; set; } | Tipo de parámetro utilizado. Si parameterType=value, se usará el valor de boolean, double, integer o string. En este caso, se espera que solo se especifique uno de {boolean, double, integer, o string}. |
| [Value](../../aspose.cells.externalconnections/connectionparameter/value/) { get; set; } | Valor numérico no entero, valor entero, valor de cadena o valor booleano para usar como parámetro de consulta. Se usa solo cuando parameterType es value. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            
            try
            {
                // Crear un parámetro de conexión mediante reflexión ya que el constructor no es público
                ConnectionParameter parameter = (ConnectionParameter)Activator.CreateInstance(typeof(ConnectionParameter), nonPublic: true);
                
                // Establecer propiedades básicas
                parameter.Name = "CustomerID";
                parameter.Type = ConnectionParameterType.Value;
                parameter.Value = "CUST1001";
                parameter.RefreshOnChange = true;
                parameter.Prompt = "Enter Customer ID:";
                
                // Mostrar información del parámetro
                Console.WriteLine($"Created parameter: {parameter.Name}");
                Console.WriteLine($"Type: {parameter.Type}");
                Console.WriteLine($"Value: {parameter.Value}");
                Console.WriteLine($"Refresh on change: {parameter.RefreshOnChange}");
                Console.WriteLine($"Prompt: {parameter.Prompt}");
                
                // Guarda el libro de trabajo
                workbook.Save("ConnectionParameterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameter: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


