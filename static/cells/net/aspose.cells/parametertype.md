##Enum ParameterType
Aspose.Cells.ParameterType enum. Represents all parameters type or return value type of function
## ParameterType enumeration
Represents all parameters' type or return value type of function.
```csharp
public enum ParameterType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Reference | `0` |  |
| Value | `1` |  |
| Array | `2` |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ParameterTypeDemo
{
public static void ParameterTypeExample()
{
// Creating a workbook and worksheet to demonstrate the usage
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Example usage of the ParameterType enum in a formula function
// Let's assume we are defining a custom function with specific parameter types
// Define an array of parameter types
ParameterType[] parameterTypes = new ParameterType[]
{
ParameterType.Reference,
ParameterType.Value,
ParameterType.Array
};
// Example function that uses these parameter types
// For instance, setting a hypothetical custom function with defined parameter types
// (Note: Custom function handling would depend on Aspose.Cells API capabilities)
// Save the workbook to demonstrate the changes
workbook.Save("ParameterTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
