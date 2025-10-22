##Metered.GetProductName
Metered method. Gets product name
## Metered.GetProductName method
Gets product name
```csharp
public string GetProductName()
```
### Return Value
product name
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MeteredMethodGetProductNameDemo
{
public static void Run()
{
// Create a metered instance
Metered metered = new Metered();
// Set metered keys (replace with actual keys)
metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");
// Get and display product name
string productName = metered.GetProductName();
Console.WriteLine("Product Name: " + productName);
// Demonstrate basic usage with a simple spreadsheet
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].PutValue("Product: " + productName);
workbook.Save("MeteredProductDemo.xlsx");
}
}
}
```
### See Also
* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
