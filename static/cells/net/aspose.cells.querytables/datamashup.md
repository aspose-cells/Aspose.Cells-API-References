##Class DataMashup
Aspose.Cells.QueryTables.DataMashup class. Represents mashup data
## DataMashup class
Represents mashup data.
```csharp
public class DataMashup
```
## Properties
| Name | Description |
| --- | --- |
| [PowerQueryFormulaParameters](../../aspose.cells.querytables/datamashup/powerqueryformulaparameters/) { get; } | (**Obsolete.**) Gets power query formula parameters. |
| [PowerQueryFormulas](../../aspose.cells.querytables/datamashup/powerqueryformulas/) { get; } | Gets all power query formulas. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.QueryTables;
using System;
public class DataMashupDemo
{
public static void DataMashupExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the DataMashup property of the workbook
DataMashup dataMashup = workbook.DataMashup;
if (dataMashup != null )
{
// Access the PowerQueryFormulas property
var powerQueryFormulas = dataMashup.PowerQueryFormulas;
// Access the PowerQueryFormulaParameters property
var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;
// Example usage: Iterate through PowerQueryFormulas
foreach (var formula in powerQueryFormulas)
{
Console.WriteLine(formula.Name);
}
// Example usage: Iterate through PowerQueryFormulaParameters
foreach (var parameter in powerQueryFormulaParameters)
{
Console.WriteLine(parameter.Name);
}
}
// Save the workbook
workbook.Save("DataMashupExample.xlsx");
workbook.Save("DataMashupExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)
