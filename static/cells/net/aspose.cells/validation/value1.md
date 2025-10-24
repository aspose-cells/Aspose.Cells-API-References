##Validation.Value1
Validation property. Represents the first value associated with the data validation
## Validation.Value1 property
Represents the first value associated with the data validation.
```csharp
public object Value1 { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyValue1Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a validation in cell A1
Validation validation = worksheet.Cells["A1"].GetValidation();
validation.Type = ValidationType.List;
// Set Value1 property with string array
validation.Value1 = new object[] { "Option1", "Option2", "Option3" };
// Get and display the validation values
object[] values = validation.Value1 as object[];
Console.WriteLine("Validation values in A1:");
foreach (object value in values)
{
Console.WriteLine(value.ToString());
}
// Create another validation in cell B1 with different values
Validation validation2 = worksheet.Cells["B1"].GetValidation();
validation2.Type = ValidationType.List;
validation2.Value1 = new object[] { "Yes", "No", "Maybe" };
// Get and display the second validation values
object[] values2 = validation2.Value1 as object[];
Console.WriteLine("\nValidation values in B1:");
foreach (object value in values2)
{
Console.WriteLine(value.ToString());
}
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
