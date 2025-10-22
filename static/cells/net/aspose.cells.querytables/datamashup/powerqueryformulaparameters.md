##DataMashup.PowerQueryFormulaParameters
DataMashup property. Gets power query formula parameters
## DataMashup.PowerQueryFormulaParameters property
Gets power query formula parameters.
```csharp
[Obsolete("Use DataMashup.PowerQueryFormulas property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PowerQueryFormulaParameterCollection PowerQueryFormulaParameters { get; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use DataMashup.PowerQueryFormulas property. This property will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;
namespace AsposeCellsExamples
{
public class DataMashupPropertyPowerQueryFormulaParametersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the DataMashup property
DataMashup dataMashup = workbook.DataMashup;
if (dataMashup != null)
{
// Access PowerQueryFormulaParameters
PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;
// Display parameter count
Console.WriteLine($"Number of parameters: {parameters.Count}");
// Iterate through parameters if any exist
foreach (PowerQueryFormulaParameter parameter in parameters)
{
Console.WriteLine($"Parameter Name: {parameter.Name}, Value: {parameter.Value}");
}
}
// Save the workbook
workbook.Save("DataMashupDemo.xlsx");
}
}
}
```
### See Also
* class [PowerQueryFormulaParameterCollection](../../powerqueryformulaparametercollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
