---
title: Metered.SetMeteredKey
second_title: Aspose.Cells for .NET API Reference
description: Metered method. Sets metered public and private key. If you purchase metered license when start application this API should be called normally this is enough. However if always fail to upload consumption data and exceed 24 hours the license will be set to evaluation status to avoid such case you should regularly check the license status if it is evaluation status call this API again
type: docs
url: /net/aspose.cells/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | String | public key |
| privateKey | String | private key |

### Examples

```csharp
// Called: metered.SetMeteredKey(publicKey, privateKey);
public static void Method_String_()
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


