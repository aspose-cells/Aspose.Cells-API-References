##WorkbookDesigner.UpdateReference
WorkbookDesigner property. Indicates if references in other worksheets will be updated
## WorkbookDesigner.UpdateReference property
Indicates if references in other worksheets will be updated.
```csharp
public bool UpdateReference { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerPropertyUpdateReferenceDemo
{
public static void Run()
{
// Create a sample dataset
DataSet ds = new DataSet();
DataTable dt = new DataTable("Products");
dt.Columns.Add("ID", typeof(int));
dt.Columns.Add("Name", typeof(string));
dt.Columns.Add("Price", typeof(decimal));
dt.Rows.Add(1, "Product A", 19.99);
dt.Rows.Add(2, "Product B", 29.99);
dt.Rows.Add(3, "Product C", 39.99);
ds.Tables.Add(dt);
// Create a workbook designer
WorkbookDesigner designer = new WorkbookDesigner();
// Set the UpdateReference property to true
designer.UpdateReference = true;
// Create a new workbook with a template
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add smart markers
worksheet.Cells["A1"].PutValue("&=Products.ID");
worksheet.Cells["B1"].PutValue("&=Products.Name");
worksheet.Cells["C1"].PutValue("&=Products.Price");
designer.Workbook = workbook;
designer.SetDataSource("Products", dt);
// Process the designer
designer.Process();
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
