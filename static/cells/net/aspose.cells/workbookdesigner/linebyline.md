##WorkbookDesigner.LineByLine
WorkbookDesigner property. Indicates whether processing the smart marker line by line
## WorkbookDesigner.LineByLine property
Indicates whether processing the smart marker line by line.
```csharp
[Obsolete("Use range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LineByLine { get; set; }
```
### Remarks
The default value is true. If False, the template file must contain a range which is named as "_CellsSmartMarkers".
NOTE: This class is now obsolete. Instead, please use range smart markers. This property will be removed 12 months later since July 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerPropertyLineByLineDemo
{
public static void Run()
{
// Create a sample workbook with smart markers
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Set up smart markers in the worksheet
ws.Cells["A1"].PutValue("&RootData.Name");
ws.Cells["A2"].PutValue("&RootData.Age");
ws.Cells["A3"].PutValue("&RootData.Department");
// Create sample data
var employee = new EmployeeData
{
Name = "John Doe",
Age = 35,
Department = "Sales"
};
List<EmployeeData> employees = new List<EmployeeData> { employee };
// Process with LineByLine set to false
WorkbookDesigner designer = new WorkbookDesigner
{
Workbook = wb,
LineByLine = false // This is the key property being demonstrated
};
designer.SetDataSource("RootData", employees);
designer.Process();
// Save the result
wb.Save("output.xlsx");
Console.WriteLine("Workbook processed with LineByLine=false. Output saved to output.xlsx");
}
}
// Simple data class for demonstration
public class EmployeeData
{
public string Name { get; set; }
public int Age { get; set; }
public string Department { get; set; }
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
