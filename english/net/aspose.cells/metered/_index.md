---
title: Class Metered
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Metered class. Provides methods to set metered key
type: docs
url: /net/aspose.cells/metered/
---
## Metered class

Provides methods to set metered key.

```csharp
public class Metered
```

## Constructors

| Name | Description |
| --- | --- |
| [Metered](metered/)() | Initializes a new instance of this class. |

## Methods

| Name | Description |
| --- | --- |
| [GetProductName](../../aspose.cells/metered/getproductname/)() | Gets the product name |
| [SetMeteredKey](../../aspose.cells/metered/setmeteredkey/)(string, string) | Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again. |
| static [GetConsumptionCredit](../../aspose.cells/metered/getconsumptioncredit/)() | Gets consumption credit |
| static [GetConsumptionQuantity](../../aspose.cells/metered/getconsumptionquantity/)() | Gets consumption file size |
| static [IsMeteredLicensed](../../aspose.cells/metered/ismeteredlicensed/)() | Check whether metered is licensed |

### Examples

In this example, an attempt will be made to set metered public and private key

```csharp
[C#]

Metered matered = new Metered();
matered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim matered As Metered = New Metered
matered.SetMeteredKey("PublicKey", "PrivateKey")
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


