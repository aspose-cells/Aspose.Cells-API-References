##ReferredAreaCollection.Item
ReferredAreaCollection property.
## ReferredAreaCollection indexer
```csharp
public ReferredArea this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index |  |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
Worksheet worksheet1 = workbook.Worksheets["Sheet1"];
Worksheet worksheet2 = workbook.Worksheets["Sheet2"];
worksheet2.Cells.CreateRange("E5:I6").Name = "someNamedRange_1";
worksheet1.Cells["A1"].Formula = "=SUM(someNamedRange_1)";
ReferredAreaCollection precedents = worksheet1.Cells["A1"].GetPrecedents();
if (precedents.Count > 0)
{
ReferredArea firstPrecedent = precedents[0]; // Using Item property via indexer
Console.WriteLine("First precedent sheet name: " + firstPrecedent.SheetName);
}
}
}
}
```
### See Also
* class [ReferredArea](../../referredarea/)
* class [ReferredAreaCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
