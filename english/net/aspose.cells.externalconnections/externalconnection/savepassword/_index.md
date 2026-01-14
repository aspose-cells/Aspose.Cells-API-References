---
title: ExternalConnection.SavePassword
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. True if the password is to be saved as part of the connection string otherwise False
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/savepassword/
---
## ExternalConnection.SavePassword property

True if the password is to be saved as part of the connection string; otherwise, False.

```csharp
public bool SavePassword { get; set; }
```

### Examples

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
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Access the first external connection (assuming one exists)
                ExternalConnection connection = workbook.DataConnections[0];

                // Display the current SavePassword value
                Console.WriteLine("Initial SavePassword value: " + connection.SavePassword);

                // Demonstrate setting the property (since it's read-write)
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Updated SavePassword value: " + connection.SavePassword);

                // Toggle the value to demonstrate setting capability
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Toggled SavePassword value: " + connection.SavePassword);

                // Save the workbook with the modified connection settings
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

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


