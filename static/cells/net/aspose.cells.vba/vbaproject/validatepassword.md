##VbaProject.ValidatePassword
VbaProject method. Validates protection password
## VbaProject.ValidatePassword method
Validates protection password.
```csharp
public bool ValidatePassword(string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| password | String | the password |
### Return Value
Whether password is the protection password of this VBA project
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VbaProjectMethodValidatePasswordWithStringDemo
{
public static void Run()
{
// Create workbook object from sample Excel file with VBA project
Workbook workbook = new Workbook("example.xlsm");
// Validate the VBA project password
bool isValid = workbook.VbaProject.ValidatePassword("test");
// Output the validation result
Console.WriteLine("Password validation result: " + isValid);
}
}
}
```
### See Also
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
