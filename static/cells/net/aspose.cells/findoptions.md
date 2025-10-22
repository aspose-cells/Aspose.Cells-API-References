##Class FindOptions
Aspose.Cells.FindOptions class. Represents find options
## FindOptions class
Represents find options.
```csharp
public class FindOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [FindOptions](findoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive/) { get; set; } | Indicates if the searched string is case sensitive. |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata/) { get; set; } | Gets or sets a value that indicates whether converting the searched string value to numeric data. |
| [IsCaseSensitive](../../aspose.cells/findoptions/iscasesensitive/) { get; set; } | (**Obsolete.**) Indicates if the searched string is case sensitive. |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset/) { get; } | Indicates whether the searched range is set. |
| [LookAtType](../../aspose.cells/findoptions/lookattype/) { get; set; } | Look at type. |
| [LookInType](../../aspose.cells/findoptions/lookintype/) { get; set; } | Look in type. |
| [RegexKey](../../aspose.cells/findoptions/regexkey/) { get; set; } | Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel. |
| [SeachOrderByRows](../../aspose.cells/findoptions/seachorderbyrows/) { get; set; } | (**Obsolete.**) Indicates whether search order by rows or columns. |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward/) { get; set; } | Whether search backward for cells. |
| [SearchNext](../../aspose.cells/findoptions/searchnext/) { get; set; } | (**Obsolete.**) Search order. True: search next. False: search previous. |
| [SearchOrderByRows](../../aspose.cells/findoptions/searchorderbyrows/) { get; set; } | Indicates whether search order by rows or columns. |
| [Style](../../aspose.cells/findoptions/style/) { get; set; } | The format to search for. |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive/) { get; set; } | Indicates whether searched cell value type should be same with the searched key. |
## Methods
| Name | Description |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange/)() | Gets and sets the searched range. |
| [SetRange](../../aspose.cells/findoptions/setrange/)(CellArea) | Sets the searched range. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FindOptionsDemo
{
public static void FindOptionsExample()
{
// Instantiate the workbook object
Workbook workbook = new Workbook("FindOptionsExample_original.xlsx");
// Get Cells collection
Cells cells = workbook.Worksheets[0].Cells;
// Instantiate FindOptions Object
FindOptions findOptions = new FindOptions();
// Create a Cells Area
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.StartColumn = 0;
ca.EndRow = 5;
ca.EndColumn = 5;
// Set cells area for find options
findOptions.SetRange(ca);
// Set searching properties
findOptions.SearchBackward = false;
findOptions.SeachOrderByRows = true;
findOptions.LookInType = LookInType.Values;
// Find the cell with 0 value
Cell cell = cells.Find(0, null, findOptions);
if (cell != null)
{
Console.WriteLine("Cell found at: " + cell.Name);
}
else
{
Console.WriteLine("Cell not found.");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
