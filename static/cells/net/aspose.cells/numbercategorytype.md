##Enum NumberCategoryType
Aspose.Cells.NumberCategoryType enum. Represents category type of cells number formatting
## NumberCategoryType enumeration
Represents category type of cell's number formatting.
```csharp
public enum NumberCategoryType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| General | `0` | General |
| Text | `1` | Text |
| Number | `2` | Number |
| Date | `3` | Date or Date and Time |
| Time | `4` | Time |
| Fraction | `5` | Fraction |
| Scientific | `6` | Scientific |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class NumberCategoryTypeDemo
{
public static void NumberCategoryTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("General");
worksheet.Cells["A2"].PutValue("Text");
worksheet.Cells["A3"].PutValue(12345);
worksheet.Cells["A4"].PutValue(DateTime.Now);
worksheet.Cells["A5"].PutValue(TimeSpan.FromHours(1.5));
worksheet.Cells["A6"].PutValue(0.75);
worksheet.Cells["A7"].PutValue(1.23E+3);
// Set number formats for the cells
worksheet.Cells["A1"].SetStyle(CreateStyle(workbook, NumberCategoryType.General));
worksheet.Cells["A2"].SetStyle(CreateStyle(workbook, NumberCategoryType.Text));
worksheet.Cells["A3"].SetStyle(CreateStyle(workbook, NumberCategoryType.Number));
worksheet.Cells["A4"].SetStyle(CreateStyle(workbook, NumberCategoryType.Date));
worksheet.Cells["A5"].SetStyle(CreateStyle(workbook, NumberCategoryType.Time));
worksheet.Cells["A6"].SetStyle(CreateStyle(workbook, NumberCategoryType.Fraction));
worksheet.Cells["A7"].SetStyle(CreateStyle(workbook, NumberCategoryType.Scientific));
// Output the number category types
Console.WriteLine("Cell A1 Number Category Type: " + worksheet.Cells["A1"].NumberCategoryType);
Console.WriteLine("Cell A2 Number Category Type: " + worksheet.Cells["A2"].NumberCategoryType);
Console.WriteLine("Cell A3 Number Category Type: " + worksheet.Cells["A3"].NumberCategoryType);
Console.WriteLine("Cell A4 Number Category Type: " + worksheet.Cells["A4"].NumberCategoryType);
Console.WriteLine("Cell A5 Number Category Type: " + worksheet.Cells["A5"].NumberCategoryType);
Console.WriteLine("Cell A6 Number Category Type: " + worksheet.Cells["A6"].NumberCategoryType);
Console.WriteLine("Cell A7 Number Category Type: " + worksheet.Cells["A7"].NumberCategoryType);
// Save the workbook
workbook.Save("NumberCategoryTypeExample.xlsx");
}
private static Style CreateStyle(Workbook workbook, NumberCategoryType numberCategoryType)
{
Style style = workbook.CreateStyle();
switch (numberCategoryType)
{
case NumberCategoryType.General:
style.Number = 0;
break;
case NumberCategoryType.Text:
style.Number = 49;
break;
case NumberCategoryType.Number:
style.Number = 1;
break;
case NumberCategoryType.Date:
style.Number = 14;
break;
case NumberCategoryType.Time:
style.Number = 21;
break;
case NumberCategoryType.Fraction:
style.Number = 9;
break;
case NumberCategoryType.Scientific:
style.Number = 11;
break;
}
return style;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
