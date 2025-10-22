##WorkbookSettings.CheckExcelRestriction
WorkbookSettings property. Whether check restriction of excel file when user modify cells related objects. For example excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValuestring if this property is true you will get an Exception. If this property is false we will accept your input string value as the cells value so that later you can output the complete string value for other file formats such as CSV. However if you have set such kind of value that is invalid for excel file format you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file
## WorkbookSettings.CheckExcelRestriction property
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.
```csharp
public bool CheckExcelRestriction { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyCheckExcelRestrictionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Disable Excel restriction checking
workbook.Settings.CheckExcelRestriction = false;
// Insert a string that exceeds normal Excel limits
string longString = new string('a', 40000);
workbook.Worksheets[0].Cells["A1"].PutValue(longString);
// Save and reload to verify the restriction is bypassed
string tempFile = Guid.NewGuid().ToString() + ".txt";
workbook.Save(tempFile, new TxtSaveOptions());
Workbook loadedWorkbook = new Workbook(tempFile, new LoadOptions { CheckExcelRestriction = false });
Console.WriteLine("String length: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue.Length);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
