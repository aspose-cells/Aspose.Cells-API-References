##Class PivotFields
Aspose.Cells.GridWeb.Data.PivotFields class. Reprents A collection of all the PivotField objects in a PivotTable report
## PivotFields class
Reprents A collection of all the [`PivotField`](../pivotfield/) objects in a PivotTable report.
```csharp
[Obsolete("This class is obsolete; use GridPivotFieldCollection instead")]
public class PivotFields : ICollection
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotfields/count/) { get; } | Gets the number of elements contained in the PivotFields instance |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotfields/issynchronized/) { get; } | Gets a value indicating whether access to the PivotFields is synchronized (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/pivotfields/item/) { get; } | Gets a PivotField by index. (2 indexers) |
| [Parent](../../aspose.cells.gridweb.data/pivotfields/parent/) { get; } | Gets the parent object for the specified object. Read-only. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotfields/syncroot/) { get; } | Gets an object that can be used to synchronize access to the PivotFields. |
## Methods
| Name | Description |
| --- | --- |
| [CopyTo](../../aspose.cells.gridweb.data/pivotfields/copyto/)(Array, int) | Copies the entire PivotField to a compatible one-dimensional Array, starting at the specified index of the target array |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotfields/getenumerator/)() | Returns an IEnumerator for the PivotFields. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotfields/indexof/)(PivotField) | Gets the index of the specified PivotField. |
### Remarks
NOTE: This class is now obsolete. please use GridPivotFieldCollection Instead. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
[C#]
//Gets PivotFields of PivotTable[0]
PivotField field1 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field1"];
PivotField field2 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field2"];
PivotField field3 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field3"];
PivotField field4 = GridWeb1.WebWorksheets.PivotTables[0].PivotFields["field4"];
//Sets Location of PivotFields
field1.Orientation = PivotFieldOrientation.RowField;
field2.Orientation = PivotFieldOrientation.RowField;
field3.Orientation = PivotFieldOrientation.ColumnField;
field4.Orientation = PivotFieldOrientation.DataField;
//Sets function of data field
field3.Function = PivotFieldFunction.Sum;
//Changes row fields order
field2.Position = 1; //Or field1.Position = 2;
[VB]
'Gets PivotFields of PivotTable[0]
Dim field1 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field1")
Dim field2 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field2")
Dim field3 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field3")
Dim field4 As PivotField =  GridWeb1.WebWorksheets.PivotTables(0).PivotFields("field4")
'Sets Location of PivotFields
field1.Orientation = PivotFieldOrientation.RowField
field2.Orientation = PivotFieldOrientation.RowField
field3.Orientation = PivotFieldOrientation.ColumnField
field4.Orientation = PivotFieldOrientation.DataField
'Sets function of data field
field3.Function = PivotFieldFunction.Sum
'Changes row fields order
field2.Position = 1 'Or field1.Position = 2;
```
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
