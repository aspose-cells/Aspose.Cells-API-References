##Cells.RemoveFormulas
Cells method. Removes all formula and replaces with the value of the formula
## Cells.RemoveFormulas method
Removes all formula and replaces with the value of the formula.
```csharp
public void RemoveFormulas()
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodRemoveFormulasDemo
{
public static void Run()
{
// Create a sample dataset
DataSet ds = new DataSet();
// Create and populate Master table
DataTable dtMaster = new DataTable("Master");
dtMaster.Columns.Add("ACCOUNT", typeof(string));
dtMaster.Columns.Add("ACCOUNT_CREATEDBY_NAME", typeof(string));
dtMaster.Rows.Add("Test_Account", "Test_user");
ds.Tables.Add(dtMaster);
// Create and populate OppLineItems table
DataTable lineItems = new DataTable("OppLineItems");
lineItems.Columns.Add("Id", typeof(int));
lineItems.Columns.Add("Name", typeof(string));
lineItems.Columns.Add("SALESPRICE", typeof(int));
lineItems.Rows.Add(1, "lineItem1", 10);
lineItems.Rows.Add(2, "lineItem2", 20);
ds.Tables.Add(lineItems);
// Create a new workbook
Workbook wkb = new Workbook();
// Use WorkbookDesigner to bind data
WorkbookDesigner designer = new WorkbookDesigner { Workbook = wkb };
designer.SetDataSource(ds);
designer.Process(false);
// Add a formula to demonstrate removal
wkb.Worksheets[0].Cells["A10"].Formula = "=SUM(C2:C3)";
// Calculate formulas first
wkb.CalculateFormula();
// Remove all formulas from the worksheet
wkb.Worksheets[0].Cells.RemoveFormulas();
// Save the workbook
wkb.Save("output.xlsx");
Console.WriteLine("Formulas removed and workbook saved successfully.");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
