##WriteProtection.RecommendReadOnly
WriteProtection property. Indicates if the Read Only Recommended option is selected
## WriteProtection.RecommendReadOnly property
Indicates if the Read Only Recommended option is selected.
```csharp
public bool RecommendReadOnly { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WriteProtectionPropertyRecommendReadOnlyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access worksheet and add some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Data");
// Set RecommendReadOnly to true
workbook.Settings.WriteProtection.RecommendReadOnly = true;
// Verify the property is set
Console.WriteLine("RecommendReadOnly: " + workbook.Settings.WriteProtection.RecommendReadOnly);
Console.WriteLine("IsWriteProtected: " + workbook.Settings.WriteProtection.IsWriteProtected);
// Save the workbook
workbook.Save("output_recommend_readonly.xlsx");
// Load the saved workbook to verify settings persist
Workbook loadedWorkbook = new Workbook("output_recommend_readonly.xlsx");
Console.WriteLine("After loading - RecommendReadOnly: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
Console.WriteLine("After loading - IsWriteProtected: " + loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
}
}
}
```
### See Also
* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
