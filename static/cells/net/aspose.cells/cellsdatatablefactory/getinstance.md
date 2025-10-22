##CellsDataTableFactory.GetInstance
CellsDataTableFactory method. Creates ICellsDataTable from given sequence of int values
## GetInstance(int[], string[]) {#getinstance_5}
Creates ICellsDataTable from given sequence of int values.
```csharp
public ICellsDataTable GetInstance(int[] vals, string[] columnNames)
```
| Parameter | Type | Description |
| --- | --- | --- |
| vals | Int32[] | int values to build table |
| columnNames | String[] | Column names of the table. Its length can only be either 1(build table by the int values vertically) or length of the int values(build table by the int values horizontally) |
### Return Value
Instance of ICellsDataTable
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsDataTableFactoryMethodGetInstanceWithInt32StringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data for the method parameters (Int32[], String[])
int[] values = new int[] { 100, 200, 300, 400, 500 };
string[] columnNames = new string[] { "Column1", "Column2", "Column3", "Column4", "Column5" };
try
{
// Create CellsDataTableFactory instance using reflection
CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
// Call GetInstance with (Int32[], String[]) parameters
ICellsDataTable dataTable = factory.GetInstance(values, columnNames);
// Output the data to worksheet
worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());
// Display some information about the created table
Console.WriteLine("Method executed successfully with parameters (Int32[], String[])");
Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
// Print column names
Console.WriteLine("Column Names:");
foreach (string colName in dataTable.Columns)
{
Console.WriteLine(colName);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
}
// Save the result
workbook.Save("CellsDataTableFactoryGetInstanceWithInt32StringDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(int[], bool) {#getinstance_4}
Creates ICellsDataTable from given sequence of int values.
```csharp
public ICellsDataTable GetInstance(int[] vals, bool vertial)
```
| Parameter | Type | Description |
| --- | --- | --- |
| vals | Int32[] | int values to build table |
| vertial | Boolean | whether build table by the int values vertiacally(true) or horizontally(false) |
### Return Value
Instance of ICellsDataTable
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsDataTableFactoryMethodGetInstanceWithInt32ArrayBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data for the method parameters (Int32[], Boolean)
int[] values = new int[] { 10, 20, 30, 40, 50 };
bool vertical = true;
try
{
// Create CellsDataTableFactory instance
CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
// Call GetInstance with (Int32[], Boolean) parameters
ICellsDataTable dataTable = factory.GetInstance(values, vertical);
// Output the data to worksheet
int row = 0;
dataTable.BeforeFirst();
while (dataTable.Next())
{
for (int col = 0; col < dataTable.Columns.Length; col++)
{
worksheet.Cells[row, col].PutValue(dataTable[col]);
}
row++;
}
Console.WriteLine("Data table created successfully from Int32[] with vertical orientation");
Console.WriteLine($"Total rows processed: {row}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
}
// Save the result
workbook.Save("CellsDataTableFactoryGetInstanceWithInt32ArrayBooleanDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(double[], string[]) {#getinstance_2}
Creates ICellsDataTable from given sequence of double values.
```csharp
public ICellsDataTable GetInstance(double[] vals, string[] columnNames)
```
| Parameter | Type | Description |
| --- | --- | --- |
| vals | Double[] | double values to build table |
| columnNames | String[] | Column names of the table. Its length can only be either 1(build table by the double values vertically) or length of the double values(build table by the double values horizontally) |
### Return Value
Instance of ICellsDataTable
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsDataTableFactoryMethodGetInstanceWithDoubleStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data for the method parameters (Double[], String[])
double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
string[] columnNames = new string[] { "Price", "Cost", "Margin", "Tax", "Total" };
try
{
// Create CellsDataTableFactory instance
CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
// Call GetInstance with (Double[], String[]) parameters
ICellsDataTable dataTable = factory.GetInstance(values, columnNames);
// Output the data to worksheet
worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());
// Display information about the created table
Console.WriteLine("Method executed successfully with parameters (Double[], String[])");
Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
// Print column names and values
Console.WriteLine("Column Names:");
foreach (string colName in dataTable.Columns)
{
Console.WriteLine(colName);
}
// Print values
dataTable.BeforeFirst();
while (dataTable.Next())
{
for (int i = 0; i < dataTable.Columns.Length; i++)
{
Console.WriteLine($"{dataTable.Columns[i]}: {dataTable[i]}");
}
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
}
// Save the result
workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleStringDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(double[], bool) {#getinstance_1}
Creates ICellsDataTable from given sequence of double values.
```csharp
public ICellsDataTable GetInstance(double[] vals, bool vertial)
```
| Parameter | Type | Description |
| --- | --- | --- |
| vals | Double[] | double values to build table |
| vertial | Boolean | whether build table by the double values vertiacally(true) or horizontally(false) |
### Return Value
Instance of ICellsDataTable
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsDataTableFactoryMethodGetInstanceWithDoubleBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data for the method parameters (Double[], Boolean)
double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
bool vertical = true;
try
{
// Create CellsDataTableFactory instance
CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
// Call GetInstance with (Double[], Boolean)
ICellsDataTable dataTable = factory.GetInstance(values, vertical);
// Output the data to worksheet
int row = 0;
dataTable.BeforeFirst();
while (dataTable.Next())
{
for (int col = 0; col < dataTable.Columns.Length; col++)
{
worksheet.Cells[row, col].PutValue(dataTable[col]);
}
row++;
}
Console.WriteLine("Data table created successfully with parameters (Double[], Boolean)");
Console.WriteLine($"Total rows processed: {row}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
}
// Save the result
workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleBooleanDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(object[], string[]) {#getinstance_10}
Creates ICellsDataTable from given sequence of objects.
```csharp
public ICellsDataTable GetInstance(object[] vals, string[] columnNames)
```
| Parameter | Type | Description |
| --- | --- | --- |
| vals | Object[] | objects to build table |
| columnNames | String[] | Column names of the table. Its length can only be either 1(build table by the objects vertically) or length of the objects(build table by the objects horizontally) |
### Return Value
Instance of ICellsDataTable
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsDataTableFactoryMethodGetInstanceWithObjectStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data for the method parameters (Object[], String[])
object[] values = new object[] { "John Doe", 35, 75000.50, DateTime.Now };
string[] columnNames = new string[] { "Name", "Age", "Salary", "Hire Date" };
try
{
// Create CellsDataTableFactory instance using reflection
CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
// Call the GetInstance method with (Object[], String[]) parameters
ICellsDataTable dataTable = factory.GetInstance(values, columnNames);
// Output the data to worksheet using ImportData instead of ImportDataTable
worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());
Console.WriteLine("Method executed successfully with parameters (Object[], String[])");
Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
}
// Save the result
workbook.Save("CellsDataTableFactoryGetInstanceWithObjectStringDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(object[][], bool, string[]) {#getinstance_11}
Creates ICellsDataTable from given sequence of objects.
```csharp
public ICellsDataTable GetInstance(object[][] vals, bool hasHeader, string[] columnNames)
```
| Parameter | Type | Description |
| --- | --- | --- |
| vals | Object[][] | objects to build table |
| hasHeader | Boolean | Indicates whether the first row is header row. |
| columnNames | String[] | Column names of the table. Its length can only be either 1(build table by the objects vertically) or length of the objects(build table by the objects horizontally) |
### Return Value
Instance of ICellsDataTable
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data for the method parameters (Object[][], Boolean, String[])
object[][] data = new object[][]
{
new object[] { "ID", "Name", "Price" },
new object[] { 1, "Laptop", 999.99 },
new object[] { 2, "Phone", 699.99 },
new object[] { 3, "Tablet", 399.99 }
};
bool hasHeader = true;
string[] columnNames = new string[] { "ProductID", "ProductName", "ProductPrice" };
try
{
// Create CellsDataTableFactory instance
CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
// Call GetInstance with (Object[][], Boolean, String[])
ICellsDataTable dataTable = factory.GetInstance(data, hasHeader, columnNames);
// Output the data to worksheet
int row = 0;
dataTable.BeforeFirst();
while (dataTable.Next())
{
for (int col = 0; col < dataTable.Columns.Length; col++)
{
worksheet.Cells[row, col].PutValue(dataTable[col]);
}
row++;
}
Console.WriteLine("Data table created successfully with parameters (Object[][], Boolean, String[])");
Console.WriteLine($"Total rows processed: {row}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
}
// Save the result
workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanStringDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(object[], bool) {#getinstance_9}
Creates ICellsDataTable from given sequence of objects.
```csharp
public ICellsDataTable GetInstance(object[] vals, bool vertial)
```
| Parameter | Type | Description |
| --- | --- | --- |
| vals | Object[] | objects to build table |
| vertial | Boolean | whether build table by the objects vertiacally(true) or horizontally(false) |
### Return Value
Instance of ICellsDataTable
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data for the method parameters (Object[], Boolean)
object[] data = new object[] { "Product", "Price", "Stock", "Available" };
bool vertical = true;
try
{
// Create CellsDataTableFactory instance using reflection
CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
// Call GetInstance with (Object[], Boolean) parameters
ICellsDataTable dataTable = factory.GetInstance(data, vertical);
// Output the data to worksheet
dataTable.BeforeFirst();
int row = 0;
while (dataTable.Next())
{
for (int col = 0; col < dataTable.Columns.Length; col++)
{
worksheet.Cells[row, col].PutValue(dataTable[col]);
}
row++;
}
Console.WriteLine("Data table created successfully with parameters (Object[], Boolean)");
Console.WriteLine($"Data orientation: {(vertical ? "Vertical" : "Horizontal")}");
Console.WriteLine($"Total items processed: {dataTable.Count}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
}
// Save the result
workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(int[]) {#getinstance_3}
```csharp
public ICellsDataTable GetInstance(int[] vals)
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(double[]) {#getinstance}
```csharp
public ICellsDataTable GetInstance(double[] vals)
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(object[]) {#getinstance_8}
```csharp
public ICellsDataTable GetInstance(object[] vals)
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(ICollection) {#getinstance_6}
Creates ICellsDataTable from given collection.
```csharp
public ICellsDataTable GetInstance(ICollection collection)
```
| Parameter | Type | Description |
| --- | --- | --- |
| collection | ICollection | the collection to build table |
### Return Value
Instance of ICellsDataTable
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections;
public class CellsDataTableFactoryMethodGetInstanceWithICollectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare an ArrayList as ICollection
ArrayList data = new ArrayList
{
new ArrayList { "Product", "Price", "Stock" },
new ArrayList { "Keyboard", 49.99, 120 },
new ArrayList { "Mouse", 29.99, 200 },
new ArrayList { "Monitor", 199.99, 35 }
};
try
{
// Create CellsDataTableFactory instance
CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
// Call GetInstance with ICollection parameter
ICellsDataTable dataTable = factory.GetInstance(data);
// Output the data to worksheet
int row = 0;
dataTable.BeforeFirst();
while (dataTable.Next())
{
for (int col = 0; col < dataTable.Columns.Length; col++)
{
worksheet.Cells[row, col].PutValue(dataTable[col]);
}
row++;
}
Console.WriteLine("Data table created successfully from ICollection");
Console.WriteLine($"Total rows processed: {row}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
}
// Save the result
workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetInstance(ICollection, bool) {#getinstance_7}
Creates ICellsDataTable from given collection.
```csharp
public ICellsDataTable GetInstance(ICollection collection, bool hasHeader)
```
| Parameter | Type | Description |
| --- | --- | --- |
| collection | ICollection | the collection to build table |
| hasHeader | Boolean | Indicates whether the first row is header |
### Return Value
Instance of ICellsDataTable
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections;
public class CellsDataTableFactoryMethodGetInstanceWithICollectionBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data collection for the method parameters (ICollection, Boolean)
ArrayList dataCollection = new ArrayList
{
new { Product = "Apple", Price = 2.5, Stock = 100 },
new { Product = "Orange", Price = 1.8, Stock = 150 },
new { Product = "Banana", Price = 0.9, Stock = 200 }
};
bool hasHeader = true;
try
{
// Create CellsDataTableFactory instance
CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
// Call GetInstance with (ICollection, Boolean) parameters
ICellsDataTable dataTable = factory.GetInstance(dataCollection, hasHeader);
// Output the data to worksheet
worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());
// Display information about the created table
Console.WriteLine("Method executed successfully with parameters (ICollection, Boolean)");
Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
// Print column names
Console.WriteLine("Column Names:");
foreach (string colName in dataTable.Columns)
{
Console.WriteLine(colName);
}
// Print values
dataTable.BeforeFirst();
while (dataTable.Next())
{
for (int i = 0; i < dataTable.Columns.Length; i++)
{
Console.WriteLine($"{dataTable.Columns[i]}: {dataTable[i]}");
}
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
}
// Save the result
workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionBooleanDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
