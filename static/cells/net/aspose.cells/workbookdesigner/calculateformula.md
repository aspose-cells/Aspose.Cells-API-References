##WorkbookDesigner.CalculateFormula
WorkbookDesigner property. Indicates whether formulas should be calculated
## WorkbookDesigner.CalculateFormula property
Indicates whether formulas should be calculated.
```csharp
public bool CalculateFormula { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerPropertyCalculateFormulaDemo
{
public static void Run()
{
// Create a sample workbook with a formula
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and formula
worksheet.Cells["A1"].PutValue("Opportunity Name");
worksheet.Cells["B1"].PutValue("Opportunity Amount");
worksheet.Cells["A2"].PutValue("=Master.Opportunity_Name");
worksheet.Cells["B2"].PutValue("=Master.Opportunity_Amount");
worksheet.Cells["C2"].Formula = "=CONCATENATE(A2,B2)";
// Create data source
DataTable dt = new DataTable("Master");
dt.Columns.Add("Opportunity_Name");
dt.Columns.Add("Opportunity_Amount");
DataRow dr = dt.NewRow();
dr["Opportunity_Name"] = "Test Deal";
dr["Opportunity_Amount"] = "$2500.00";
dt.Rows.Add(dr);
// Process the designer with CalculateFormula enabled
WorkbookDesigner designer = new WorkbookDesigner(workbook);
designer.SetDataSource(dt);
designer.CalculateFormula = true; // This will calculate formulas after data binding
designer.Process();
// Output the result
Console.WriteLine("Formula result: " + worksheet.Cells["C2"].StringValue);
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
