##Metered.GetConsumptionQuantity
Metered method. Gets consumption file size
## Metered.GetConsumptionQuantity method
Gets consumption file size
```csharp
public static decimal GetConsumptionQuantity()
```
### Return Value
consumption quantity
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class MeteredMethodGetConsumptionQuantityDemo
{
public static void Run()
{
// Create a metered instance
Metered metered = new Metered();
try
{
// Set metered keys (replace with actual keys in real usage)
metered.SetMeteredKey("your-public-key", "your-private-key");
// Get consumption quantity
decimal consumptionQuantity = Metered.GetConsumptionQuantity();
// Display the result
Console.WriteLine($"Consumption Quantity: {consumptionQuantity}");
// Create a workbook to demonstrate the metered usage
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to show the workbook is functional
worksheet.Cells["A1"].PutValue("Metered Consumption Demo");
worksheet.Cells["A2"].PutValue($"Consumption Quantity: {consumptionQuantity}");
// Save the workbook
workbook.Save("MeteredConsumptionDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error in metered operation: {ex.Message}");
}
}
}
}
```
### See Also
* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
