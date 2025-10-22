##WorkbookDesigner.UpdateEmptyStringAsNull
WorkbookDesigner property. If TRUE Null will be inserted if the value is
## WorkbookDesigner.UpdateEmptyStringAsNull property
If TRUE, Null will be inserted if the value is "";
```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerPropertyUpdateEmptyStringAsNullDemo
{
public static void Run()
{
// Create a sample DataSet with empty strings
DataSet ds = new DataSet();
DataTable dt = new DataTable("Products");
dt.Columns.Add("Name");
dt.Columns.Add("Price");
dt.Rows.Add("Laptop", "");
dt.Rows.Add("", "999.99");
ds.Tables.Add(dt);
// Create a workbook with designer markers
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("&=$Products.Name");
worksheet.Cells["B1"].PutValue("&=$Products.Price");
// Initialize WorkbookDesigner and set properties
WorkbookDesigner designer = new WorkbookDesigner();
designer.Workbook = workbook;
designer.UpdateEmptyStringAsNull = true; // This is the key property being demonstrated
// Set data source and process
designer.SetDataSource(ds.Tables["Products"]);
designer.Process();
// Verify results
Console.WriteLine("A1 value: " + worksheet.Cells["A1"].StringValue); // Should show "Laptop"
Console.WriteLine("B1 value: " + worksheet.Cells["B1"].StringValue); // Should show empty (null)
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
