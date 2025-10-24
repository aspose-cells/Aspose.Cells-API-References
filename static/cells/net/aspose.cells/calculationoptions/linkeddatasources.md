##CalculationOptions.LinkedDataSources
CalculationOptions property. Specifies the data sources for external links used in formulas
## CalculationOptions.LinkedDataSources property
Specifies the data sources for external links used in formulas.
```csharp
public Workbook[] LinkedDataSources { get; set; }
```
### Remarks
Like [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/). The match of those workbooks with external links is determined by [`FileName`](../../workbook/filename/) and [`DataSource`](../../externallink/datasource/). So please make sure [`FileName`](../../workbook/filename/) has been specified with the proper value(generally it should be same with corresponding [`DataSource`](../../externallink/datasource/)) for every workbook so they can be linked as expected.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationOptionsPropertyLinkedDataSourcesDemo
{
public static void Run()
{
// Create external workbook with data
Workbook wbExt = new Workbook();
wbExt.Worksheets[0].Cells["A2"].PutValue(100);
wbExt.Worksheets.Add("Sheet2").Cells["A2"].PutValue(200);
// Add named ranges in external workbook
int nameIndex1 = wbExt.Worksheets.Names.Add("Sheet1!ExtNamedRange1");
wbExt.Worksheets.Names[nameIndex1].RefersTo = "=Sheet1!$A$2";
int nameIndex2 = wbExt.Worksheets.Names.Add("Sheet2!ExtNamedRange2");
wbExt.Worksheets.Names[nameIndex2].RefersTo = "=Sheet2!$A$2";
int nameIndex3 = wbExt.Worksheets.Names.Add("GlobalNamedRange");
wbExt.Worksheets.Names[nameIndex3].RefersTo = "=Sheet1!$A$2";
// Create main workbook
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Set formulas that reference external workbook
sheet.Cells["A1"].Formula = "=[External.xlsx]Sheet1!$A$2";
sheet.Cells["A2"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!$A$2\")";
sheet.Cells["A3"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!ExtNamedRange1\")";
sheet.Cells["A4"].Formula = "=INDIRECT(\"[External.xlsx]!GlobalNamedRange\")";
// Calculate formulas using LinkedDataSources
CalculationOptions options = new CalculationOptions();
options.LinkedDataSources = new Workbook[] { wbExt };
Console.WriteLine("Before calculation:");
PrintCellValues(sheet);
wb.CalculateFormula(options);
Console.WriteLine("\nAfter calculation:");
PrintCellValues(sheet);
}
private static void PrintCellValues(Worksheet sheet)
{
for (int i = 0; i < 4; i++)
{
Console.WriteLine($"Cell A{i+1}: {sheet.Cells[$"A{i+1}"].StringValue}");
}
}
}
}
```
### See Also
* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
