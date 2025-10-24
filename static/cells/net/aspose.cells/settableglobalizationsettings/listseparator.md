##SettableGlobalizationSettings.ListSeparator
SettableGlobalizationSettings property. Gets the separator for list parameters of function ...etc
## SettableGlobalizationSettings.ListSeparator property
Gets the separator for list, parameters of function, ...etc.
```csharp
public override char ListSeparator { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsPropertyListSeparatorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SettableGlobalizationSettings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Display the current ListSeparator value (default is comma in most locales)
Console.WriteLine("Current ListSeparator value: " + settings.ListSeparator);
// Set a new ListSeparator value (e.g., semicolon)
settings.SetListSeparator(';');
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
// Demonstrate the effect of ListSeparator in formula parsing
worksheet.Cells["A1"].PutValue("Test");
worksheet.Cells["A2"].PutValue("Data");
// Create a formula that uses the list separator
worksheet.Cells["A3"].Formula = "=CONCATENATE(A1,A2)";
// The formula will use the custom list separator when parsed
Console.WriteLine("Formula with custom separator: " + worksheet.Cells["A3"].Formula);
// Save the workbook
workbook.Save("PropertyListSeparatorDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
