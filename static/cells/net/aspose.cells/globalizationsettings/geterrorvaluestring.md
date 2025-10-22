##GlobalizationSettings.GetErrorValueString
GlobalizationSettings method. Gets the display string value for cells error value
## GlobalizationSettings.GetErrorValueString method
Gets the display string value for cell's error value
```csharp
public virtual string GetErrorValueString(string err)
```
| Parameter | Type | Description |
| --- | --- | --- |
| err | String | error values such as #VALUE!,#NAME? |
### Return Value
By default returns the error value itself
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class GlobalizationSettingsMethodGetErrorValueStringWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set custom globalization settings
workbook.Settings.GlobalizationSettings = new CustomErrorGlobalizationSettings();
// Create error scenario: Division by zero
Cell cell = worksheet.Cells["A1"];
cell.Formula = "=1/0";  // This will generate #DIV/0! error
try
{
workbook.CalculateFormula();
string errorValue = cell.DisplayStringValue;
Console.WriteLine($"Error display value: {errorValue}");
Console.WriteLine("Method executed successfully - see custom error mapping");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
}
workbook.Save("MethodGetErrorValueStringDemo.xlsx");
}
}
public class CustomErrorGlobalizationSettings : GlobalizationSettings
{
public override string GetErrorValueString(string err)
{
// Custom error value mappings
return err switch
{
"#DIV/0!" => "Custom Division Error",
"#VALUE!" => "Custom Type Mismatch",
"#NAME?" => "Custom Identifier Error",
_ => base.GetErrorValueString(err)
};
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
