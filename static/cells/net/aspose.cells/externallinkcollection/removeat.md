##ExternalLinkCollection.RemoveAt
ExternalLinkCollection method. Removes the specified external link from the workbook
## RemoveAt(int) {#removeat}
Removes the specified external link from the workbook.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the external link to be removed. |
### Remarks
When removing the external link, all formulas that reference to it will be removed too because the references become invalid.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a workbook with sample external links
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample external links
worksheet.Cells["A1"].Formula = "='C:/ExternalFiles/File1.xlsx'!Sheet1!A1";
worksheet.Cells["A2"].Formula = "='C:/ExternalFiles/File2.xlsx'!Sheet1!A1";
worksheet.Cells["A3"].Formula = "='C:/ImportantFiles/File3.xlsx'!Sheet1!A1";
// Get external links collection
ExternalLinkCollection elc = workbook.Worksheets.ExternalLinks;
Console.WriteLine("Initial external links count: " + elc.Count);
// Remove external links that don't contain "ImportantFiles" in their path
for (int i = elc.Count - 1; i >= 0; i--)
{
if (!elc[i].DataSource.Contains("ImportantFiles"))
{
elc.RemoveAt(i);
}
}
Console.WriteLine("Remaining external links count: " + elc.Count);
Console.WriteLine("Remaining external link path: " + elc[0].DataSource);
}
}
}
```
### See Also
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RemoveAt(int, bool) {#removeat_1}
Removes the specified external link from the workbook.
```csharp
public void RemoveAt(int index, bool updateReferencesAsLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the external link to be removed. |
| updateReferencesAsLocal | Boolean | Whether update all references of given external link to reference of current workbook itself. Check [`Clear`](../clear/) to get more details about this parameter. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkCollectionMethodRemoveAtWithInt32BooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
// Add some external links
ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;
elc.Add("externallink1.xlam", new string[] { "externallink1.xlam" });
elc.Add("externallink2.xlam", new string[] { "externallink2.xlam" });
elc.Add("externallink3.xlam", new string[] { "externallink3.xlam" });
elc.Add("externallink4.xlam", new string[] { "externallink4.xlam" });
// Add some formulas referencing these external links
Worksheet ws = wb.Worksheets[0];
for (int i = 0; i < 4; i++)
{
for (int j = 0; j < 3; j++)
{
ws.Cells[j, i].Formula = $"=externallink{i+1}.xlam!customfunc{j+1}()";
}
}
Console.WriteLine($"Initial external links count: {elc.Count}");
Console.WriteLine("Formulas before removal:");
for (int i = 0; i < 4; i++)
{
Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
}
// Remove at index 1 with updateReferences=true
elc.RemoveAt(1, true);
Console.WriteLine($"\nAfter removing at index 1 (updateReferences=true):");
Console.WriteLine($"External links count: {elc.Count}");
Console.WriteLine("Updated formulas:");
for (int i = 0; i < 3; i++)
{
Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
}
// Remove at index 0 with updateReferences=false
elc.RemoveAt(0, false);
Console.WriteLine($"\nAfter removing at index 0 (updateReferences=false):");
Console.WriteLine($"External links count: {elc.Count}");
Console.WriteLine("Formulas (should be cleared where references were removed):");
for (int i = 0; i < 2; i++)
{
Console.WriteLine($"Cell A{i+1}: Has formula? {ws.Cells[0, i].IsFormula}");
}
}
}
}
```
### See Also
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
