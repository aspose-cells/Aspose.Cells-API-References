##WorksheetCollection.RegisterAddInFunction
WorksheetCollection method. Adds addin function into the workbook
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}
Adds addin function into the workbook
```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```
| Parameter | Type | Description |
| --- | --- | --- |
| addInFile | String | the file contains the addin functions |
| functionName | String | the addin function name |
| lib | Boolean | whether the given addin file is in the directory or sub-directory of Workbook Add-In library. This flag takes effect and makes difference when given addInFile is of relative path: true denotes the path is relative to Add-In library and false denotes the path is relative to this Workbook. |
### Return Value
ID of the data which contains given addin function
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodRegisterAddInFunctionWithStringStringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Get the first worksheet
Worksheet sheet = wb.Worksheets[0];
// Set sample file paths (these would need to exist in your environment)
string addInFile1 = Path.Combine("AddIns", "MyAddIn1.xlam");
string addInFile2 = Path.Combine("AddIns", "MyAddIn2.xlam");
// Register add-in functions with different parameters
int id1 = wb.Worksheets.RegisterAddInFunction(addInFile1, "MY_UDF1", false);
int id2 = wb.Worksheets.RegisterAddInFunction(addInFile2, "MY_UDF2", true);
// Use the registered functions in cells
sheet.Cells["A1"].Formula = "=MY_UDF1()";
sheet.Cells["A2"].Formula = "=MY_UDF2()";
// Save the workbook
wb.Save("RegisterAddInFunctionDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RegisterAddInFunction(int, string) {#registeraddinfunction_1}
Adds addin function into the workbook
```csharp
public string RegisterAddInFunction(int id, string functionName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| id | Int32 | ID of the data which contains addin functions, can be got by the first call of `RegisterAddInFunction` for the same addin file. |
| functionName | String | the addin function name |
### Return Value
URL of the addin file which contains addin functions
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodRegisterAddInFunctionWithInt32StringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Register first add-in function and get its ID
int functionId = workbook.Worksheets.RegisterAddInFunction("externallink1.xlam", "customfunc1", false);
// Register second add-in function using the same ID
workbook.Worksheets.RegisterAddInFunction(functionId, "customfunc2");
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Use the registered functions in formulas
cells["A1"].Formula = "=customfunc1()";
cells["A2"].Formula = "=customfunc2()";
// Save the workbook
workbook.Save("RegisterAddInFunctionDemo.xlsx");
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
