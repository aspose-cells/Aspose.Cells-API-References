##WorkbookDesigner.Process
WorkbookDesigner method. Processes the smart markers and populates the data source values
## Process(Range, bool) {#process_1}
Processes the smart markers and populates the data source values.
```csharp
[Obsolete("Use Range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Process(Range range, bool isPreserved)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range to be processed |
| isPreserved | Boolean | True if the unrecognized smart marker is preserved. |
### Remarks
NOTE: This class is now obsolete. Instead, please use Range smart markers. This property will be removed 12 months later since July 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodProcessWithRangeBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Access first worksheet
Worksheet sheet = wb.Worksheets[0];
// Create sample data in cells
sheet.Cells["A1"].PutValue("Name");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["A2"].PutValue("&=$Name");
sheet.Cells["B2"].PutValue("&=$Value");
// Create workbook designer
WorkbookDesigner designer = new WorkbookDesigner();
designer.Workbook = wb;
// Create JSON data source
string jsonData = "{'Name':'Test Product','Value':100.50}";
designer.SetJsonDataSource("Data", jsonData);
// Process specific range with smart markers
Aspose.Cells.Range range = sheet.Cells.CreateRange("A2:B2");
range.Name = "_CellsSmartMarkers";
// Process the range (true = process only this range)
designer.Process(range, true);
// Save the result
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Process() {#process}
Processes the smart markers and populates the data source values.
```csharp
public void Process()
```
### Examples
```csharp
using System;
using System.Collections;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodProcessDemo
{
public static void Run()
{
// Create a workbook from template file
Workbook workbook = new Workbook("example.xlsx");
WorkbookDesigner designer = new WorkbookDesigner(workbook);
// Prepare data source
ArrayList persons = new ArrayList();
Person person1 = new Person("John Doe", 30);
person1.FOTO = File.ReadAllBytes("1.jpg");
persons.Add(person1);
Person person2 = new Person("Jane Smith", 28);
person2.FOTO = File.ReadAllBytes("1.jpg");
persons.Add(person2);
// Set data source and process
designer.SetDataSource("Datos", persons);
designer.Process();
// Save the result
workbook.Save("output.xlsx");
}
}
public class Person
{
public string Name { get; set; }
public int Age { get; set; }
public byte[] FOTO { get; set; }
public Person(string name, int age)
{
Name = name;
Age = age;
}
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Process(bool) {#process_2}
Processes the smart markers and populates the data source values.
```csharp
public void Process(bool isPreserved)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isPreserved | Boolean | True if the unrecognized smart marker is preserved. |
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodProcessWithBooleanDemo
{
public static void Run()
{
// Initialize workbook and load template
Workbook workbook = new Workbook("example.xlsx");
// Create sample data directly instead of loading from JSON
ABC_1_Data data = new ABC_1_Data
{
Directors = new List<Director>
{
new Director { DRFNAME2 = "DRFNAME2" }
}
};
// Set up smart markers
workbook.Worksheets[0].Cells.CreateRange("A13:K19").Name = "_CellsSmartMarkers";
// Prepare data sources
List<ABC_1_Data> listData = new List<ABC_1_Data> { data };
// Process workbook designer
WorkbookDesigner designer = new WorkbookDesigner
{
Workbook = workbook,
LineByLine = false
};
designer.SetDataSource("RootData", listData);
designer.SetDataSource("Directors", data.Directors);
// Process with boolean parameter
designer.Process(true);
// Save result
workbook.Save("output.xlsx");
}
}
// Sample data classes
public class ABC_1_Data
{
public List<Director> Directors { get; set; }
}
public class Director
{
public string DRFNAME2 { get; set; }
}
}
```
### See Also
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Process(int, bool) {#process_3}
Processes the smart markers and populates the data source values.
```csharp
public void Process(int sheetIndex, bool isPreserved)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Worksheet index. |
| isPreserved | Boolean | True if the unrecognized smart marker is preserved. |
### Remarks
This method works on worksheet level.
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookDesignerMethodProcessWithInt32BooleanDemo
{
public static void Run()
{
// Create a workbook from source file
Workbook workbook = new Workbook("example.xlsx");
// Export data from worksheet to DataTable
Worksheet worksheet = workbook.Worksheets["Data"];
DataTable dataTable = worksheet.Cells.ExportDataTable(
0, 0,
worksheet.Cells.MaxDataRow,
worksheet.Cells.MaxDataColumn + 1,
new ExportTableOptions {
CheckMixedValueType = true,
ExportColumnName = true
});
dataTable.TableName = "Table";
// Create workbook designer and set data source
WorkbookDesigner designer = new WorkbookDesigner();
designer.Workbook = workbook;
designer.SetDataSource(dataTable);
// Process the designer with parameters (Int32, Boolean)
designer.Process(0, true);
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
