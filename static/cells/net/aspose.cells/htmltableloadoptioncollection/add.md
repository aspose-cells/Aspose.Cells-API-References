##HtmlTableLoadOptionCollection.Add
HtmlTableLoadOptionCollection method. Adds one HtmlTableLoadOption into this collection
## Add(HtmlTableLoadOption) {#add}
Adds one HtmlTableLoadOption into this collection.
```csharp
public int Add(HtmlTableLoadOption item)
```
| Parameter | Type | Description |
| --- | --- | --- |
| item | HtmlTableLoadOption | one HtmlTableLoadOption |
### Return Value
the index of the added item
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionCollectionMethodAddWithHtmlTableLoadOptionDemo
{
public static void Run()
{
// Create HTML load options
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Add table load options
HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
tableLoadOption1.Id = "table1";
loadOptions.TableLoadOptions.Add(tableLoadOption1);
HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
tableLoadOption2.Id = "table2";
tableLoadOption2.TargetSheetIndex = 1;
loadOptions.TableLoadOptions.Add(tableLoadOption2);
// Load workbook with options
Workbook workbook = new Workbook("input.html", loadOptions);
// Save the output
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(int) {#add_1}
Add a HtmlTableLoadOption to the list.
```csharp
public int Add(int tableIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | Int32 | Table index |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionCollectionMethodAddWithInt32Demo
{
public static void Run()
{
// Create HtmlLoadOptions
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Access the HtmlTableLoadOptionCollection instance
HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;
// Add a new HtmlTableLoadOption by table index
int index = tableLoadOptions.Add(0);
// Access the added HtmlTableLoadOption
HtmlTableLoadOption option = tableLoadOptions[index];
option.TableToListObject = true;
// Create a workbook and load HTML with options
Workbook workbook = new Workbook("input.html", loadOptions);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(string) {#add_4}
Add a HtmlTableLoadOption to the list.
```csharp
public int Add(string tableId)
```
| Parameter | Type | Description |
| --- | --- | --- |
| tableId | String | Table ID |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionCollectionMethodAddWithStringDemo
{
public static void Run()
{
// Create HtmlLoadOptions
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Access the HtmlTableLoadOptionCollection instance
HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;
// Add a new HtmlTableLoadOption by table id
int index = tableLoadOptions.Add("mainTable");
// Access the added HtmlTableLoadOption
HtmlTableLoadOption option = tableLoadOptions[index];
option.TableToListObject = true;
option.TargetSheetIndex = 0;
// Create workbook and load HTML with options
Workbook workbook = new Workbook("input.html", loadOptions);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(int, int) {#add_2}
Add a HtmlTableLoadOption to the list.
```csharp
public int Add(int tableIndex, int targetSheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | Int32 | Table index |
| targetSheetIndex | Int32 | The target index of worksheet in Excel |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Demo
{
public static void Run()
{
// Create HTML load options
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Add tables by index with target sheet index
loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 to sheet index 2
loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 to sheet index 0
loadOptions.TableLoadOptions.Add(2, 1); // Table index 2 to sheet index 1
// Load HTML file with the specified options
Workbook workbook = new Workbook("input.html", loadOptions);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(string, int) {#add_5}
Add a HtmlTableLoadOption to the list.
```csharp
public int Add(string tableId, int targetSheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| tableId | String | Table ID |
| targetSheetIndex | Int32 | The target index of worksheet in Excel |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Demo
{
public static void Run()
{
// Create HtmlLoadOptions
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Access the HtmlTableLoadOptionCollection instance
HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;
// Add a new HtmlTableLoadOption by table id and target sheet index
int index = tableLoadOptions.Add("tableId", 1);
// Create a workbook and load HTML with options
Workbook workbook = new Workbook("input.html", loadOptions);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(int, int, int) {#add_3}
Add a HtmlTableLoadOption to the list.
```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | Int32 | Table index |
| targetSheetIndex | Int32 | The target index of worksheet in Excel |
| originalSheetIndex | Int32 | The original index of worksheet in the html |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Int32Demo
{
public static void Run()
{
// Create HtmlLoadOptions
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Access the HtmlTableLoadOptionCollection
HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;
// Add a table with index 1, target sheet index 1, and original sheet index 0
int addedIndex = tableLoadOptions.Add(1, 1, 0);
// Create a workbook and load HTML with options
Workbook workbook = new Workbook("input.html", loadOptions);
// Save the result
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(string, int, int) {#add_6}
Add a HtmlTableLoadOption to the list.
```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| tableId | String | Table ID |
| targetSheetIndex | Int32 | The target index of worksheet in Excel |
| originalSheetIndex | Int32 | The original index of worksheet in the html |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;
// Demonstrate Add method with (String, Int32, Int32) parameters
int addedIndex = tableLoadOptions.Add("sampleTable", 1, 0);
HtmlTableLoadOption option = tableLoadOptions[addedIndex];
option.TableToListObject = true;
// Load HTML file (replace with actual file path)
workbook = new Workbook("input.html", loadOptions);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
