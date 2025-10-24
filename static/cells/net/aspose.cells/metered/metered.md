##Metered.Metered
Metered constructor. Initializes a new instance of this class
## Metered constructor
Initializes a new instance of this class.
```csharp
public Metered()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MeteredMethodCtorDemo
{
public static void Run()
{
// Create an instance using the constructor
Metered metered = new Metered();
// Set metered license
metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");
// Create a simple workbook to demonstrate functionality
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Metered License Demo");
// Save the workbook
workbook.Save("MeteredDemoOutput.xlsx");
Console.WriteLine("Demo completed successfully.");
}
}
}
```
### See Also
* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
