##WorkbookDesigner.WorkbookDesigner
WorkbookDesigner constructor. Initializes a new instance of the WorkbookDesigner class
## WorkbookDesigner() {#constructor}
Initializes a new instance of the [`WorkbookDesigner`](../) class.
```csharp
public WorkbookDesigner()
```
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodCtorDemo
{
public static void Run()
{
// Create a new WorkbookDesigner using the constructor
WorkbookDesigner designer = new WorkbookDesigner();
// Create sample data source
List<Level> levels = new List<Level>();
levels.Add(new Level("r1", "c1"));
levels.Add(new Level("r2", "c2"));
levels.Add(new Level("r3", "c3"));
// Create a new workbook and set it as designer's workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set markers in the worksheet
worksheet.Cells["A1"].PutValue("&Level.Name");
worksheet.Cells["B1"].PutValue("&Level.Value");
// Set the workbook to designer
designer.Workbook = workbook;
// Set data source and process
designer.SetDataSource("Level", levels);
designer.Process();
// Save the result
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
public class Level
{
public string Name { get; set; }
public string Value { get; set; }
public Level(string name, string value)
{
Name = name;
Value = value;
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## WorkbookDesigner(Workbook) {#constructor_1}
Initializes a new instance of the [`WorkbookDesigner`](../) class.
```csharp
public WorkbookDesigner(Workbook workbook)
```
| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The template workbook file. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodCtorWithWorkbookDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data in cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["A2"].PutValue("&=$ds.object.object1.name");
// Create JSON data source
string jsonData = "{\"object\": {\"object1\": {\"name\": \"John Doe\"}}}";
// Initialize WorkbookDesigner with the workbook
WorkbookDesigner designer = new WorkbookDesigner(workbook);
// Set JSON data source
designer.SetJsonDataSource("ds", jsonData);
// Process the designer
designer.Process();
// Output the result
Console.WriteLine("Processed value: " + worksheet.Cells["A2"].StringValue);
}
}
}
```
### See Also
* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
