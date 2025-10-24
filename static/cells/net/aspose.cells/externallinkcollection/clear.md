##ExternalLinkCollection.Clear
ExternalLinkCollection method. Removes all external links
## Clear() {#clear}
Removes all external links.
```csharp
public void Clear()
```
### Remarks
When removing external links, all formulas that reference to them will be removed too because the references become invalid.
### See Also
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Clear(bool) {#clear_1}
Removes all external links.
```csharp
public void Clear(bool updateReferencesAsLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Whether update all references of external links in formulas to references of current workbook itself. |
### Remarks
If references are required to be updated, those references of external links in formulas will be changed to current workbook when it is possible. For example, one cell's original formula is "='externalsource.xlam'!customfunction()", after removing external links, the formula will become "=customfunction()"; When the original formula is "='[externalsource.xlam]Sheet1'!$A$1", according to whether there is one sheet with name "Sheet1" in current workbook: if true, the formula will become "=Sheet1!$A$1"; if false, the formula will become "=#REF!$A$1". If references are not required to be updated, all formulas with references to external links will be removed too because those references become invalid.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkCollectionMethodClearWithBooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add some external links
ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
Console.WriteLine("External links count before clear: " + externalLinks.Count);
// Clear with updateReferences = true
externalLinks.Clear(true);
Console.WriteLine("External links count after clear (updateReferences=true): " + externalLinks.Count);
// Add links again
externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
// Clear with updateReferences = false
externalLinks.Clear(false);
Console.WriteLine("External links count after clear (updateReferences=false): " + externalLinks.Count);
}
}
}
```
### See Also
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
