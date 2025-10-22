##PivotTableCollection.Add
PivotTableCollection method. Adds a new PivotTable
## Add(string, string, string) {#add_5}
Adds a new PivotTable.
```csharp
public int Add(string sourceData, string destCellName, string tableName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data for the new PivotTable cache. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
### Return Value
The new added cache index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableCollectionMethodAddWithStringStringStringDemo
{
public static void Run()
{
// Create a workbook from source CSV
Workbook workbook = new Workbook();
Worksheet sourceSheet = workbook.Worksheets[0];
sourceSheet.Name = "SourceData";
// Add sample data
sourceSheet.Cells["A1"].PutValue("Category");
sourceSheet.Cells["B1"].PutValue("Value");
sourceSheet.Cells["A2"].PutValue("A");
sourceSheet.Cells["B2"].PutValue(10);
sourceSheet.Cells["A3"].PutValue("B");
sourceSheet.Cells["B3"].PutValue(20);
sourceSheet.Cells["A4"].PutValue("A");
sourceSheet.Cells["B4"].PutValue(30);
// Create pivot table worksheet
Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
// Get the source data range
Aspose.Cells.Range sourceRange = sourceSheet.Cells.MaxDisplayRange;
string sourceData = String.Format("=SourceData!{0}", sourceRange.Address);
// Add pivot table using String, String, String parameters
PivotTableCollection pivotTables = pivotSheet.PivotTables;
int pivotIndex = pivotTables.Add(sourceData, "A1", "MyPivotTable");
// Configure pivot table
PivotTable pivotTable = pivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Save the workbook
workbook.Save("PivotTableDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## Add(string, string, string, bool) {#add_6}
Adds a new PivotTable.
```csharp
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data for the new PivotTable cache. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | Boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |
### Return Value
The new added cache index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableCollectionMethodAddWithStringStringStringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = worksheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 15;
cells["A4"].Value = "Banana";
cells["B4"].Value = 20;
// Define parameters for Add method
string sourceData = "A1:B4";
string destCellName = "E5";
string tableName = "FruitPivotTable";
bool useSameSource = true;
try
{
// Call the Add method with parameters (String, String, String, Boolean)
int index = worksheet.PivotTables.Add(sourceData, destCellName, tableName, useSameSource);
Console.WriteLine($"Pivot table added successfully at index: {index}");
Console.WriteLine($"Pivot table name: {worksheet.PivotTables[index].Name}");
Console.WriteLine($"Pivot table location: {worksheet.PivotTables[index].TableRange1}");
// Configure the pivot table
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the workbook
workbook.Save("PivotTableAddDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## Add(string, int, int, string) {#add_2}
Adds a new PivotTable.
```csharp
public int Add(string sourceData, int row, int column, string tableName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
### Return Value
The new added cache index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableCollectionMethodAddWithStringInt32Int32StringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet for data
Worksheet dataWorksheet = workbook.Worksheets[0];
dataWorksheet.Name = "Data";
// Add sample data
dataWorksheet.Cells["A1"].PutValue("Category");
dataWorksheet.Cells["B1"].PutValue("Product");
dataWorksheet.Cells["C1"].PutValue("Sales");
dataWorksheet.Cells["A2"].PutValue("Electronics");
dataWorksheet.Cells["B2"].PutValue("Laptop");
dataWorksheet.Cells["C2"].PutValue(1000);
dataWorksheet.Cells["A3"].PutValue("Electronics");
dataWorksheet.Cells["B3"].PutValue("Phone");
dataWorksheet.Cells["C3"].PutValue(800);
dataWorksheet.Cells["A4"].PutValue("Furniture");
dataWorksheet.Cells["B4"].PutValue("Chair");
dataWorksheet.Cells["C4"].PutValue(200);
// Add a worksheet for pivot table
Worksheet pivotWorksheet = workbook.Worksheets.Add("PivotTable");
// Add pivot table using the Add method with (String, Int32, Int32, String) parameters
string pivotDataRange = "Data!A1:C4";
int row = 0;
int column = 0;
string tableName = "SalesPivotTable";
int pivotIndex = pivotWorksheet.PivotTables.Add(pivotDataRange, row, column, tableName);
// Access the pivot table
PivotTable pivotTable = pivotWorksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Set consolidation function
pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
// Refresh and calculate pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## Add(string, int, int, string, bool) {#add_3}
Adds a new PivotTable.
```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | Boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |
### Return Value
The new added cache index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Product");
cells["B1"].PutValue("Region");
cells["C1"].PutValue("Sales");
cells["A2"].PutValue("Product1");
cells["B2"].PutValue("North");
cells["C2"].PutValue(1000);
cells["A3"].PutValue("Product2");
cells["B3"].PutValue("South");
cells["C3"].PutValue(2000);
cells["A4"].PutValue("Product3");
cells["B4"].PutValue("East");
cells["C4"].PutValue(3000);
// Define the data range
string sourceData = "A1:C4";
try
{
// Call the Add method with parameters: (String sourceData, Int32 row, Int32 column, String tableName, Boolean useSameSource)
int index = worksheet.PivotTables.Add(sourceData, 6, 0, "PivotTable1", false);
Console.WriteLine("Pivot table added successfully at index: " + index);
// Access the newly created pivot table
PivotTable pivotTable = worksheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableAddDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## Add(string, int, int, string, bool, bool) {#add_4}
Adds a new PivotTable.
```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource,
bool isXlsClassic)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | Boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |
| isXlsClassic | Boolean | Indicates whether add classic pivot table of Excel 97-2003. |
### Return Value
The new added cache index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanBDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Product");
cells["B1"].PutValue("Region");
cells["C1"].PutValue("Sales");
cells["A2"].PutValue("Product1");
cells["B2"].PutValue("North");
cells["C2"].PutValue(1000);
cells["A3"].PutValue("Product2");
cells["B3"].PutValue("South");
cells["C3"].PutValue(2000);
cells["A4"].PutValue("Product3");
cells["B4"].PutValue("East");
cells["C4"].PutValue(3000);
cells["A5"].PutValue("Product4");
cells["B5"].PutValue("West");
cells["C5"].PutValue(4000);
// Define the source data range
string sourceData = "A1:C5";
try
{
// Call the Add method with parameters (String, Int32, Int32, String, Boolean, Boolean)
int index = worksheet.PivotTables.Add(
sourceData,    // String sourceData
3,            // Int32 row - pivot table will start at row 3
0,            // Int32 column - pivot table will start at column 0
"PivotTable1", // String tableName
false,        // Boolean useSameSource
false         // Boolean isXlsClassic
);
Console.WriteLine("Pivot table added successfully at index: " + index);
// Configure the pivot table
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableAddDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## Add(string, string, string, bool, bool) {#add_7}
Adds a new PivotTable.
```csharp
public int Add(string sourceData, string cell, string tableName, bool useSameSource,
bool isXlsClassic)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| cell | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
| useSameSource | Boolean | Indicates whether using same data source when another existing pivot table has used this data source. If the property is true, it will save memory. |
| isXlsClassic | Boolean | Indicates whether add classic pivot table of Excel 97-2003. |
### Return Value
The new added cache index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableCollectionMethodAddWithStringStringStringBooleanBooleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Category");
cells["B1"].PutValue("Product");
cells["C1"].PutValue("Sales");
for (int i = 2; i <= 10; i++)
{
cells["A" + i].PutValue("Cat" + (i % 3 + 1));
cells["B" + i].PutValue("Prod" + i);
cells["C" + i].PutValue(i * 100);
}
// Add pivot table with specified parameters
int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E1", "SalesPivot", false, false);
Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
// Configure pivot table
pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0); // Category as row
pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2); // Sum of Sales
workbook.Save("PivotTableDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## Add(PivotTable, string, string) {#add_1}
Adds a new PivotTable based on another PivotTable.
```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | The source pivotTable. |
| destCellName | String | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
### Return Value
The new added PivotTable index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableCollectionMethodAddWithPivotTableStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
Cells cells = worksheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 5;
cells["A4"].Value = "Banana";
cells["B4"].Value = 7;
// Create a pivot table from the data range
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable sourcePivotTable = pivotTables[pivotIndex];
try
{
// Call the Add method with parameters (PivotTable, String, String)
int newPivotIndex = pivotTables.Add(sourcePivotTable, "E10", "PivotTable2");
Console.WriteLine($"New pivot table added at index: {newPivotIndex}");
// Save the workbook to show the effect
workbook.Save("PivotTableCollectionMethodAddWithPivotTableStringStringDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
}
}
}
```
### See Also
* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## Add(PivotTable, int, int, string) {#add}
Adds a new PivotTable based on another PivotTable.
```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | The source pivotTable. |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
### Return Value
The new added PivotTable index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
Cells cells = worksheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 5;
cells["A4"].Value = "Banana";
cells["B4"].Value = 7;
// Create a source pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("A1:B4", "C3", "SourcePivotTable");
PivotTable sourcePivotTable = pivotTables[pivotIndex];
sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
try
{
// Call the Add method with parameters (PivotTable, Int32, Int32, String)
int newPivotIndex = pivotTables.Add(sourcePivotTable, 10, 5, "NewPivotTable");
Console.WriteLine($"New pivot table added at index: {newPivotIndex}");
// Save the workbook to show the effect
workbook.Save("PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
}
}
}
```
### See Also
* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## Add(string[], bool, PivotPageFields, string, string) {#add_9}
Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.
```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields,
string destCellName, string tableName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String[] | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored. |
| pageFields | PivotPageFields | The pivot page field items. |
| destCellName | String | destCellName The name of the new PivotTable report. |
| tableName | String | the name of the new PivotTable report. |
### Return Value
The new added PivotTable index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = worksheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Region";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Product1";
cells["B2"].Value = "North";
cells["C2"].Value = 1000;
cells["A3"].Value = "Product2";
cells["B3"].Value = "South";
cells["C3"].Value = 2000;
cells["A4"].Value = "Product3";
cells["B4"].Value = "East";
cells["C4"].Value = 3000;
// Define data range
string[] sourceData = { "A1:C4" };
bool isAutoPage = true;
PivotPageFields pageFields = new PivotPageFields();
string destCellName = "E5";
string tableName = "PivotTable1";
try
{
// Call the Add method with specified parameters
int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, destCellName, tableName);
Console.WriteLine($"Pivot table added successfully at index: {index}");
// Access the newly created pivot table
PivotTable pivotTable = worksheet.PivotTables[index];
// Configure pivot table fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the workbook
workbook.Save("PivotTableAddDemo.xlsx");
}
}
}
```
### See Also
* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## Add(string[], bool, PivotPageFields, int, int, string) {#add_8}
Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.
```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row,
int column, string tableName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | String[] | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Whether auto create a single page field. If true,the following param pageFields will be ignored |
| pageFields | PivotPageFields | The pivot page field items. |
| row | Int32 | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | Int32 | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | String | The name of the new PivotTable report. |
### Return Value
The new added PivotTable index.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = worksheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Region";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Product1";
cells["B2"].Value = "North";
cells["C2"].Value = 1000;
cells["A3"].Value = "Product2";
cells["B3"].Value = "South";
cells["C3"].Value = 2000;
cells["A4"].Value = "Product3";
cells["B4"].Value = "East";
cells["C4"].Value = 3000;
cells["A5"].Value = "Product1";
cells["B5"].Value = "West";
cells["C5"].Value = 4000;
cells["A6"].Value = "Product2";
cells["B6"].Value = "North";
cells["C6"].Value = 5000;
// Define parameters for Add method
string[] sourceData = { "A1:C6" };
bool isAutoPage = true;
PivotPageFields pageFields = new PivotPageFields();
int row = 8;
int column = 1;
string tableName = "PivotTable1";
try
{
// Call the Add method with specified parameters
int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, row, column, tableName);
Console.WriteLine($"Pivot table added successfully at index: {index}");
// Configure the pivot table
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh data
pivotTable.RefreshData();
pivotTable.CalculateData();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Add method: {ex.Message}");
}
// Save the result
workbook.Save("PivotTableAddDemo.xlsx");
}
}
}
```
### See Also
* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
