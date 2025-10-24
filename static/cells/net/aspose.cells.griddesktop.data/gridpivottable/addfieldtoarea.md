##GridPivotTable.AddFieldToArea
GridPivotTable method. Adds the field to the specific area
## AddFieldToArea(GridPivotFieldType, int) {#addfieldtoarea}
Adds the field to the specific area.
```csharp
public int AddFieldToArea(GridPivotFieldType fieldType, int baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | GridPivotFieldType | The fields area type. |
| baseFieldIndex | Int32 | The field index in the base fields. |
### Return Value
The field position in the specific fields.
### See Also
* enum [GridPivotFieldType](../../gridpivotfieldtype/)
* class [GridPivotTable](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## AddFieldToArea(GridPivotFieldType, string) {#addfieldtoarea_1}
Adds the field to the specific area.
```csharp
public int AddFieldToArea(GridPivotFieldType fieldType, string fieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | GridPivotFieldType | The fields area type. |
| fieldName | String | The name in the base fields. |
### Return Value
The field position in the specific fields.If there is no field named as it, return -1.
### See Also
* enum [GridPivotFieldType](../../gridpivotfieldtype/)
* class [GridPivotTable](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
