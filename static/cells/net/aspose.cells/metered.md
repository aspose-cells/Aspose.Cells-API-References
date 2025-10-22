##Class Metered
Aspose.Cells.Metered class. Provides methods to set metered key
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
| [GetProductName](../../aspose.cells/metered/getproductname/)() | Gets product name |
| [SetMeteredKey](../../aspose.cells/metered/setmeteredkey/)(string, string) | Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again. |
| static [GetConsumptionCredit](../../aspose.cells/metered/getconsumptioncredit/)() | Gets consumption credit |
| static [GetConsumptionQuantity](../../aspose.cells/metered/getconsumptionquantity/)() | Gets consumption file size |
| static [IsMeteredLicensed](../../aspose.cells/metered/ismeteredlicensed/)() | Check whether metered is licensed |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class MeteredDemo
{
public static void MeteredExample()
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
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
