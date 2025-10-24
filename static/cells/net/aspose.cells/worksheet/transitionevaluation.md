##Worksheet.TransitionEvaluation
Worksheet property. Indicates whether the Transition Formula Evaluation Lotus compatibility option is enabled
## Worksheet.TransitionEvaluation property
Indicates whether the Transition Formula Evaluation (Lotus compatibility) option is enabled.
```csharp
public bool TransitionEvaluation { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyTransitionEvaluationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set TransitionEvaluation property
worksheet.TransitionEvaluation = true;
// Display the property value
Console.WriteLine("TransitionEvaluation: " + worksheet.TransitionEvaluation);
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook to verify the property
Workbook loadedWorkbook = new Workbook("output.xlsx");
Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
Console.WriteLine("Loaded TransitionEvaluation: " + loadedWorksheet.TransitionEvaluation);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
