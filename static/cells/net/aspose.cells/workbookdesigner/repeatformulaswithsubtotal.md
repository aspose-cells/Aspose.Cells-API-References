##WorkbookDesigner.RepeatFormulasWithSubtotal
WorkbookDesigner property. Indicates whether repeating formulas with subtotal row
## WorkbookDesigner.RepeatFormulasWithSubtotal property
Indicates whether repeating formulas with subtotal row.
```csharp
public bool RepeatFormulasWithSubtotal { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerPropertyRepeatFormulasWithSubtotalDemo
{
public static void Run()
{
// Create a sample DataTable
DataTable dt = new DataTable("products1");
dt.Columns.Add("ProductID", typeof(int));
dt.Columns.Add("ProductName", typeof(string));
dt.Columns.Add("UnitPrice", typeof(decimal));
dt.Columns.Add("Quantity", typeof(int));
// Add sample data
dt.Rows.Add(1, "Product A", 10.5m, 5);
dt.Rows.Add(2, "Product B", 15.2m, 3);
dt.Rows.Add(3, "Product C", 8.7m, 7);
// Create a new workbook with a template formula
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set up template with smart markers and formula
worksheet.Cells["A1"].PutValue("&=$ProductID");
worksheet.Cells["B1"].PutValue("&=$ProductName");
worksheet.Cells["C1"].PutValue("&=$UnitPrice");
worksheet.Cells["D1"].PutValue("&=$Quantity");
worksheet.Cells["E1"].PutValue("=SUM(C2:D2)"); // Formula to be repeated
// Create designer and set RepeatFormulasWithSubtotal
WorkbookDesigner designer = new WorkbookDesigner(workbook);
designer.RepeatFormulasWithSubtotal = true;
designer.SetDataSource(dt);
// Process the template
designer.Process();
// Verify the formula was repeated for each row
Console.WriteLine("Formula in E2: " + worksheet.Cells["E2"].Formula);
Console.WriteLine("Formula in E3: " + worksheet.Cells["E3"].Formula);
Console.WriteLine("Formula in E4: " + worksheet.Cells["E4"].Formula);
// Save the result
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
