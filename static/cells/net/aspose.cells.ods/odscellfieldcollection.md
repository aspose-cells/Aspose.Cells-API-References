##Class OdsCellFieldCollection
Aspose.Cells.Ods.OdsCellFieldCollection class. Represents the fields of ODS
## OdsCellFieldCollection class
Represents the fields of ODS.
```csharp
public class OdsCellFieldCollection : CollectionBase<OdsCellField>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.ods/odscellfieldcollection/item/) { get; } | Gets the field by the index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.ods/odscellfieldcollection/add/)(int, int, OdsCellFieldType, string) | Adds a field. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(OdsCellField) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(OdsCellField, IComparer&lt;OdsCellField&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, OdsCellField, IComparer&lt;OdsCellField&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(OdsCellField) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(OdsCellField[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(OdsCellField[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, OdsCellField[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;OdsCellField&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;OdsCellField&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;OdsCellField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;OdsCellField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;OdsCellField&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;OdsCellField&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;OdsCellField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;OdsCellField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;OdsCellField&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;OdsCellField&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(OdsCellField) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(OdsCellField, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(OdsCellField, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(OdsCellField) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(OdsCellField, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(OdsCellField, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [UpdateFieldsValue](../../aspose.cells.ods/odscellfieldcollection/updatefieldsvalue/)() | Update fields value to the cells. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
public class OdsCellFieldCollectionDemo
{
public static void OdsCellFieldCollectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Access the OdsCellFieldCollection
OdsCellFieldCollection odsCellFields = cells.OdsCellFields;
// Add fields to the OdsCellFieldCollection
int fieldIndex1 = odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
int fieldIndex2 = odsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);
int fieldIndex3 = odsCellFields.Add(2, 2, OdsCellFieldType.Title, null);
// Update fields value to the cells
odsCellFields.UpdateFieldsValue();
// Save the workbook
workbook.Save("OdsCellFieldCollectionExample.ods");
return;
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [OdsCellField](../odscellfield/)
* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)
