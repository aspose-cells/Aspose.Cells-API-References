---
title: ConnectionParameterCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ConnectionParameterCollection property. Gets the ConnectionParameter element at the specified index
type: docs
url: /net/aspose.cells.externalconnections/connectionparametercollection/item/
---
## ConnectionParameterCollection indexer (1 of 2)

Gets the [`ConnectionParameter`](../../connectionparameter/) element at the specified index.

```csharp
public ConnectionParameter this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Get the first external connection
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Get the parameters collection
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Check if there are any parameters before accessing
                if (parameters.Count > 0)
                {
                    // Demonstrate reading the Item property
                    ConnectionParameter firstParam = parameters[0];
                    Console.WriteLine($"Parameter type: {firstParam.GetType().Name}");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Save the workbook
                workbook.Save("ConnectionParameterItemDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ConnectionParameterCollection indexer (2 of 2)

Gets the [`ConnectionParameter`](../../connectionparameter/) element with the specified name.

```csharp
public ConnectionParameter this[string connParamName] { get; }
```

| Parameter | Description |
| --- | --- |
| connParamName | connection parameter name |

### Return Value

The element with the specified name.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Get the first external connection
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Get the parameters collection
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Check if there are existing parameters to demonstrate Item property
                if (parameters.Count == 0)
                {
                    Console.WriteLine("No parameters in collection to demonstrate Item property");
                    return;
                }
                
                // Get the name of the first parameter to use for demonstration
                string firstParamName = parameters[0].Name;
                
                // Demonstrate reading the Item property by name
                ConnectionParameter retrievedParam = parameters[firstParamName];
                
                if (retrievedParam != null)
                {
                    Console.WriteLine($"Retrieved parameter name: {retrievedParam.Name}");
                }
                else
                {
                    Console.WriteLine("Parameter not found");
                }
                
                // Save the workbook
                workbook.Save("ConnectionParameterItemDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


