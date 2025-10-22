##Interface ICellsDataTable
Aspose.Cells.ICellsDataTable interface. Represents data table
## ICellsDataTable interface
Represents data table.
```csharp
public interface ICellsDataTable
```
## Properties
| Name | Description |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | Gets the columns' name. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | Gets the count of the records. -1 for unknown records count. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | Gets the data stored in the column specified by index. (2 indexers) |
## Methods
| Name | Description |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | Move the cursor to the front of this object, just before the first row. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | Moves the cursor down one row from its current position. |
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassICellsDataTableDemo
{
public static void Run()
{
Workbook wb = new Workbook();
ArrayList dataLists = new ArrayList();
ArrayList list1 = new ArrayList();
list1.AddRange(new object[] { "Name", "Age", "Gender" });
ArrayList list2 = new ArrayList();
list2.AddRange(new object[] { "Alice", 30, "Female" });
ArrayList list3 = new ArrayList();
list3.AddRange(new object[] { "Bob", 25, "Male" });
ArrayList list4 = new ArrayList();
list4.AddRange(new object[] { "Charlie", 35, "Male" });
dataLists.Add(list1);
dataLists.Add(list2);
dataLists.Add(list3);
dataLists.Add(list4);
ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
Console.WriteLine("First worksheet A2 value: " + wb.Worksheets[0].Cells["A2"].StringValue);
wb.Worksheets.Add();
wb.Worksheets[1].Cells.ImportArrayList(dataLists, 0, 0, true);
Console.WriteLine("Second worksheet A3 value: " + wb.Worksheets[1].Cells["A3"].StringValue);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
