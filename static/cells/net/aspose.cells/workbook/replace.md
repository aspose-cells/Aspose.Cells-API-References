##Workbook.Replace
Workbook method. Replaces a cells value with a new string
## Replace(string, string) {#replace_7}
Replaces a cell's value with a new string.
```csharp
public int Replace(string placeHolder, string newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodReplaceWithStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("Apple Orange");
// Replace all occurrences of "Apple" with "Mango"
workbook.Replace("Apple", "Mango");
// Save the workbook
workbook.Save("ReplaceDemo.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Replace(string, int) {#replace_4}
Replaces a cell's value with a new integer.
```csharp
public int Replace(string placeHolder, int newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | Int32 | Integer value to replace |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodReplaceWithStringInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet and add some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("OriginalValue");
worksheet.Cells["A2"].PutValue("OriginalValue");
worksheet.Cells["A3"].PutValue("OriginalValue");
// Replace all occurrences of "OriginalValue" with integer 100
workbook.Replace("OriginalValue", 100);
// Save the workbook
workbook.Save("ReplacedWorkbook.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Replace(string, double) {#replace_2}
Replaces a cell's value with a new double.
```csharp
public int Replace(string placeHolder, double newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | Double | Double value to replace |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodReplaceWithStringDoubleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Put some sample data in cells
worksheet.Cells["A1"].PutValue("AnOldValue");
worksheet.Cells["A2"].PutValue("AnotherOldValue");
worksheet.Cells["A3"].PutValue("AnOldValue");
// Replace text with double value
double newValue = 100.0;
workbook.Replace("AnOldValue", newValue);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Replace(string, string[], bool) {#replace_9}
Replaces a cell's value with a new string array.
```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValues | String[] | String array to replace |
| isVertical | Boolean | True - Vertical, False - Horizontal |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodReplaceWithStringStringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to cells
worksheet.Cells["A1"].PutValue("AnOldValue");
worksheet.Cells["A2"].PutValue("AnOldValue");
worksheet.Cells["A3"].PutValue("AnOldValue");
// Define new values to replace with
string[] newValues = new string[] { "Tom", "Alice", "Jerry" };
// Replace all occurrences of "AnOldValue" with the new values
workbook.Replace("AnOldValue", newValues, true);
// Save the workbook
workbook.Save("ReplaceDemo.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Replace(string, int[], bool) {#replace_5}
Replaces cells' values with an integer array.
```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValues | Int32[] | Integer array to replace |
| isVertical | Boolean | True - Vertical, False - Horizontal |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodReplaceWithStringInt32ArrayBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to cells
worksheet.Cells["A1"].PutValue("OldValue");
worksheet.Cells["A2"].PutValue("OldValue");
worksheet.Cells["A3"].PutValue("OtherValue");
// Define replacement values
int[] newValues = new int[] { 1, 2, 3 };
// Replace "OldValue" with the array of integers
workbook.Replace("OldValue", newValues, true);
// Save the workbook
workbook.Save("ReplaceDemoOutput.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Replace(string, double[], bool) {#replace_3}
Replaces cells' values with a double array.
```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValues | Double[] | Double array to replace |
| isVertical | Boolean | True - Vertical, False - Horizontal |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodReplaceWithStringDoubleBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("AnOldValue");
worksheet.Cells["A2"].PutValue("AnOldValue");
worksheet.Cells["A3"].PutValue("AnOldValue");
// Define replacement values
double[] newValues = new double[] { 1.23, 2.56, 3.14159 };
// Replace all occurrences of "AnOldValue" with the new values
workbook.Replace("AnOldValue", newValues, true);
// Save the workbook
workbook.Save("ReplaceDemoOutput.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Replace(string, DataTable) {#replace_6}
Replaces cells' values with data from a DataTable.
```csharp
public int Replace(string placeHolder, DataTable insertTable)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| insertTable | DataTable | DataTable to replace |
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodReplaceWithStringDataTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a sample DataTable
DataTable dataTable = new DataTable("Customers");
dataTable.Columns.Add("ID", typeof(int));
dataTable.Columns.Add("Name", typeof(string));
dataTable.Columns.Add("City", typeof(string));
// Add sample data to the DataTable
dataTable.Rows.Add(1, "John Doe", "New York");
dataTable.Rows.Add(2, "Jane Smith", "London");
dataTable.Rows.Add(3, "Mike Johnson", "Paris");
// Add some text to worksheet that will be replaced
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("CustomerData");
// Replace the text with DataTable
workbook.Replace("CustomerData", dataTable);
// Save the workbook
workbook.Save("Output.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Replace(bool, object) {#replace}
Replaces cells' values with new data.
```csharp
public int Replace(bool boolValue, object newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | Boolean | The boolean value to be replaced. |
| newValue | Object | New value. Can be string, integer, double or DateTime value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorkbookMethodReplaceWithBooleanObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some cells with boolean values
worksheet.Cells["A1"].PutValue(true);
worksheet.Cells["A2"].PutValue(false);
worksheet.Cells["A3"].PutValue(true);
try
{
// Call the Replace method to replace all 'true' values with "REPLACED"
int replacements = workbook.Replace(true, "REPLACED");
Console.WriteLine($"Replaced {replacements} occurrences of 'true' with 'REPLACED'");
// Display the results
Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Replace method: {ex.Message}");
}
// Save the result
workbook.Save("WorkbookMethodReplaceWithBooleanObjectDemo.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Replace(int, object) {#replace_1}
Replaces cells' values with new data.
```csharp
public int Replace(int intValue, object newValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| intValue | Int32 | The integer value to be replaced. |
| newValue | Object | New value. Can be string, integer, double or DateTime value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorkbookMethodReplaceWithInt32ObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some cells with integer values to be replaced
worksheet.Cells["A1"].PutValue(100);
worksheet.Cells["A2"].PutValue(200);
worksheet.Cells["A3"].PutValue(100);
try
{
// Call the Replace method with parameters (Int32, Object)
int replacements = workbook.Replace(100, "ReplacedValue");
Console.WriteLine($"Replaced {replacements} occurrences of the value 100");
// Display the worksheet content after replacement
Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Replace method: {ex.Message}");
}
// Save the result
workbook.Save("WorkbookMethodReplaceWithInt32ObjectDemo.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Replace(string, string, ReplaceOptions) {#replace_8}
Replaces a cell's value with a new string.
```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |
| options | ReplaceOptions | The replace options |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodReplaceWithStringStringReplaceOptionsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Hello World");
sheet.Cells["A2"].PutValue("Hello Aspose");
sheet.Cells["A3"].PutValue("Goodbye World");
ReplaceOptions options = new ReplaceOptions
{
CaseSensitive = false,
MatchEntireCellContents = false
};
int replacedCount = workbook.Replace("Hello", "Hi", options);
Console.WriteLine($"Replacements made: {replacedCount}");
workbook.Save("ReplaceDemo.xlsx");
}
}
}
```
### See Also
* class [ReplaceOptions](../../replaceoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
