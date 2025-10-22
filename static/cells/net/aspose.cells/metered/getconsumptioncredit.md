##Metered.GetConsumptionCredit
Metered method. Gets consumption credit
## Metered.GetConsumptionCredit method
Gets consumption credit
```csharp
public static decimal GetConsumptionCredit()
```
### Return Value
consumption quantity
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class MeteredMethodGetConsumptionCreditDemo
{
public static void Run()
{
// Create an instance of Metered class
Metered metered = new Metered();
try
{
// Call GetConsumptionCredit method as static
decimal consumptionCredit = Metered.GetConsumptionCredit();
// Display the result
Console.WriteLine($"Current consumption credit: {consumptionCredit}");
// Create a simple workbook to demonstrate the effect (though GetConsumptionCredit doesn't modify workbook)
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add the consumption credit info to the worksheet
worksheet.Cells["A1"].PutValue("Consumption Credit:");
worksheet.Cells["B1"].PutValue(consumptionCredit.ToString());
// Save the workbook
workbook.Save("MeteredGetConsumptionCreditDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error getting consumption credit: {ex.Message}");
}
}
}
}
```
### See Also
* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
