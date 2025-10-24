##ErrorCheckOptionCollection.Item
ErrorCheckOptionCollection property. Gets ErrorCheckOption object by the given index
## ErrorCheckOptionCollection indexer
Gets [`ErrorCheckOption`](../../errorcheckoption/) object by the given index.
```csharp
public ErrorCheckOption this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index |
### Return Value
Return [`ErrorCheckOption`](../../errorcheckoption/) object
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ErrorCheckOptionCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;
int optionIdx = opts.Add();
// Demonstrate Item property usage
ErrorCheckOption opt = opts[optionIdx];
opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
opt.AddRange(CellArea.CreateCellArea("A1", "B3"));
workbook.Save("ErrorCheckOptionDemo.xlsx");
}
}
}
```
### See Also
* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
