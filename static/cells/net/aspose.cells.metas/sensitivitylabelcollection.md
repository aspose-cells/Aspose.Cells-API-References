##Class SensitivityLabelCollection
Aspose.Cells.Metas.SensitivityLabelCollection class. Represents the list of sensitivity labels
## SensitivityLabelCollection class
Represents the list of sensitivity labels.
```csharp
public class SensitivityLabelCollection : CollectionBase<SensitivityLabel>
```
## Constructors
| Name | Description |
| --- | --- |
| [SensitivityLabelCollection](sensitivitylabelcollection/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.metas/sensitivitylabelcollection/add/)(string, bool, SensitivityLabelAssignmentType, string, SensitivityLabelMarkType) | Adds a sensitivity label. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SensitivityLabel) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SensitivityLabel, IComparer&lt;SensitivityLabel&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, SensitivityLabel, IComparer&lt;SensitivityLabel&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(SensitivityLabel) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SensitivityLabel[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SensitivityLabel[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, SensitivityLabel[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;SensitivityLabel&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;SensitivityLabel&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SensitivityLabel) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SensitivityLabel, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SensitivityLabel, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SensitivityLabel) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SensitivityLabel, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SensitivityLabel, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Metas;
using System;
public class MetasClassSensitivityLabelCollectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of the SensitivityLabelCollection class
SensitivityLabelCollection labels = new SensitivityLabelCollection();
// Add sensitivity labels with different configurations
int index1 = labels.Add(
id: "cb353f78-2f72-4d20-a5ca-ee47c4a5e7e1",
isEnabled: true,
methodType: SensitivityLabelAssignmentType.Standard,
siteId: "contoso.sharepoint.com",
markType: SensitivityLabelMarkType.Header);
int index2 = labels.Add(
id: "e48007e5-f9ac-4f63-9edc-6ab9a312688f",
isEnabled: false,
methodType: SensitivityLabelAssignmentType.Privileged,
siteId: "contoso.sharepoint.com",
markType: SensitivityLabelMarkType.Footer);
// Apply the labels to workbook metadata
// Using CustomDocumentProperties instead since BuiltInDocumentProperties doesn't support SensitivityLabels
workbook.CustomDocumentProperties.Add("SensitivityLabels", labels.ToString());
// Save the workbook with sensitivity labels
workbook.Save("SensitivityLabelCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [SensitivityLabel](../sensitivitylabel/)
* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)
