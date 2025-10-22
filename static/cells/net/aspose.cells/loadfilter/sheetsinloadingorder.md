##LoadFilter.SheetsInLoadingOrder
LoadFilter property. Specifies the sheetsindices and order to be loaded. Default is null that denotes to load all sheets in the default order in template file. If not null and some sheets index is not in the returned array then the sheet will not be loaded
## LoadFilter.SheetsInLoadingOrder property
Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default order in template file. If not null and some sheet's index is not in the returned array, then the sheet will not be loaded.
```csharp
public virtual int[] SheetsInLoadingOrder { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LoadFilterPropertySheetsInLoadingOrderDemo
{
public static void Run()
{
// Create a new workbook with multiple sheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Create a custom load filter
LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.All);
// Display the default SheetsInLoadingOrder (null means load all sheets)
Console.WriteLine("Initial SheetsInLoadingOrder is null: " + (loadFilter.SheetsInLoadingOrder == null));
// Create a template file to demonstrate loading with custom sheet order
workbook.Save("Template.xlsx");
// Create load options with our custom filter
LoadOptions loadOptions = new LoadOptions();
loadOptions.LoadFilter = loadFilter;
// Load the workbook with default settings (all sheets)
Workbook loadedWorkbook1 = new Workbook("Template.xlsx", loadOptions);
Console.WriteLine("Sheets loaded with default filter: " + loadedWorkbook1.Worksheets.Count);
// Create a new filter with specific sheet loading order
LoadFilter orderedFilter = new LoadFilter(LoadDataFilterOptions.All)
{
// Note: SheetsInLoadingOrder is read-only, so we need to create a new filter
// with the desired order in the constructor or through other means
// This demonstrates the limitation of the property being read-only
};
// Since SheetsInLoadingOrder is read-only, we'll need to subclass LoadFilter
// to demonstrate custom sheet loading order
CustomLoadFilter customFilter = new CustomLoadFilter(new int[] { 2, 0 }); // Load Sheet3 first, then Sheet1
LoadOptions customLoadOptions = new LoadOptions();
customLoadOptions.LoadFilter = customFilter;
// Load workbook with custom sheet order
Workbook loadedWorkbook2 = new Workbook("Template.xlsx", customLoadOptions);
Console.WriteLine("Sheets loaded with custom filter: " + loadedWorkbook2.Worksheets.Count);
Console.WriteLine("First sheet in custom order: " + loadedWorkbook2.Worksheets[0].Name);
}
}
// Custom LoadFilter implementation to demonstrate SheetsInLoadingOrder functionality
public class CustomLoadFilter : LoadFilter
{
private readonly int[] _sheetsOrder;
public CustomLoadFilter(int[] sheetsOrder) : base(LoadDataFilterOptions.All)
{
_sheetsOrder = sheetsOrder;
}
public override int[] SheetsInLoadingOrder => _sheetsOrder;
}
}
```
### See Also
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
