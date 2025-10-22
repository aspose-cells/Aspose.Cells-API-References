##Class PivotField
Aspose.Cells.GridWeb.Data.PivotField class. Represents a field in a PivotTable report. The PivotField object is a member of the PivotFields collection.  NOTE This class is now obsolete. Instead please use GridPivotField. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced
## PivotField class
Represents a field in a PivotTable report. The PivotField object is a member of the [`PivotFields`](../pivotfields/) collection.  NOTE: This class is now obsolete. Instead, please use GridPivotField. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced.
```csharp
[Obsolete("This class is obsolete; use GridPivotField instead")]
public class PivotField
```
## Properties
| Name | Description |
| --- | --- |
| [Caption](../../aspose.cells.gridweb.data/pivotfield/caption/) { get; set; } | The label text for the pivot field show in report. By default show the name. |
| [FieldItems](../../aspose.cells.gridweb.data/pivotfield/fielditems/) { get; } | Gets the data of the specified field. |
| [Function](../../aspose.cells.gridweb.data/pivotfield/function/) { get; set; } | Represents function used to summarize the PivotTable field (data fields only). The default function is Count. |
| [Name](../../aspose.cells.gridweb.data/pivotfield/name/) { get; } | Gets the name. |
| [Orientation](../../aspose.cells.gridweb.data/pivotfield/orientation/) { get; set; } | Represents The location of the field in the specified PivotTable report. |
| [Position](../../aspose.cells.gridweb.data/pivotfield/position/) { get; set; } | Represents Position of the field (first, second, third, and so on) among all the fields in its orientation (Rows, Columns, Pages). you shall call the get method after calling of Pivottable.DataBind |
| [SortOrder](../../aspose.cells.gridweb.data/pivotfield/sortorder/) { get; set; } | Represents the order used to sort the specified PivotTable field. |
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
