---
title: Metered.GetProductName
second_title: Aspose.Cells for .NET API Reference
description: Metered method. Gets product name
type: docs
url: /net/aspose.cells/metered/getproductname/
---
## Metered.GetProductName method

Gets product name

```csharp
public string GetProductName()
```

### Return Value

product name

### Examples

```csharp
// Called: string productName = metered.GetProductName();
public static void Method_GetProductName()
        {
            // Create an instance of the Metered class
            Metered metered = new Metered();

            // Set the metered key
            string publicKey = &quot;YourPublicKey&quot;;
            string privateKey = &quot;YourPrivateKey&quot;;
            metered.SetMeteredKey(publicKey, privateKey);

            // Get and display the product name
            string productName = metered.GetProductName();
            Console.WriteLine(&quot;Product Name: &quot; + productName);

            // Additional code to demonstrate how the instance might be used
            // For example, creating a workbook and saving it
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue(&quot;Hello, Aspose.Cells!&quot;);

            workbook.Save(&quot;MeteredExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


