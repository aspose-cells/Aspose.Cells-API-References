##WorksheetCollection.SensitivityLabels
WorksheetCollection property. Represents all sensitivity labels
## WorksheetCollection.SensitivityLabels property
Represents all sensitivity labels.
```csharp
public SensitivityLabelCollection SensitivityLabels { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metas;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertySensitivityLabelsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the worksheet collection
WorksheetCollection worksheets = workbook.Worksheets;
// Add a sensitivity label
int index = worksheets.SensitivityLabels.Add(
"{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", // ID
true,                                       // IsEnabled
SensitivityLabelAssignmentType.Standard,     // AssignmentType
"contoso-site",                             // SiteId
SensitivityLabelMarkType.Header              // MarkType
);
// Verify the added label
SensitivityLabel label = worksheets.SensitivityLabels[index];
Console.WriteLine($"Label added - ID: {label.Id}, SiteID: {label.SiteId}");
// Save the workbook
workbook.Save("SensitivityLabelsDemo.xlsx");
}
}
}
```
### See Also
* class [SensitivityLabelCollection](../../../aspose.cells.metas/sensitivitylabelcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
