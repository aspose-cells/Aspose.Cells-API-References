---
title: Metered.Metered
second_title: Aspose.Cells for .NET API Reference
description: Metered constructor. Initializes a new instance of this class
type: docs
url: /net/aspose.cells/metered/metered/
---
## Metered constructor

Initializes a new instance of this class.

```csharp
public Metered()
```

### Examples

```csharp
// Called: Metered metered = new Metered();
public static void Metered_Constructor()
        {
            // Create an instance of the Metered class
            Metered metered = new Metered();

            // Set the metered key
            string publicKey = "YourPublicKey";
            string privateKey = "YourPrivateKey";
            metered.SetMeteredKey(publicKey, privateKey);

            // Get and display the product name
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Additional code to demonstrate how the instance might be used
            // For example, creating a workbook and saving it
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            workbook.Save("MeteredExample.xlsx");

            return;
        }
```

### See Also

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


