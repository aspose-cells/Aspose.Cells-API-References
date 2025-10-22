##WorkbookSettings.WriteProtection
WorkbookSettings property. Provides access to the workbook write protection options
## WorkbookSettings.WriteProtection property
Provides access to the workbook write protection options.
```csharp
public WriteProtection WriteProtection { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWriteProtectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set write protection properties
workbook.Settings.WriteProtection.Password = "test123";
workbook.Settings.WriteProtection.Author = "John Doe";
workbook.Settings.WriteProtection.RecommendReadOnly = true;
// Save the workbook
string outputPath = "WriteProtectionDemo.xlsx";
workbook.Save(outputPath);
// Load the saved workbook to verify properties
Workbook loadedWorkbook = new Workbook(outputPath);
// Output the write protection properties
Console.WriteLine("Author: " + loadedWorkbook.Settings.WriteProtection.Author);
Console.WriteLine("ReadOnly Recommended: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
}
}
}
```
### See Also
* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
