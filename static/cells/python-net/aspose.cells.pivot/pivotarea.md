##PivotArea class
## PivotArea class
Presents the selected area of the PivotTable.
The PivotArea type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self, table)`](/cells/python-net/aspose.cells.pivot/pivotarea/__init__/#aspose.cells.pivot.pivottable) | Presents the selected area of the PivotTable. |
### Properties
| Property | Description |
| :- | :- |
| [filters](/cells/python-net/aspose.cells.pivot/pivotarea/filters) | Gets all filters for this PivotArea. |
| [only_data](/cells/python-net/aspose.cells.pivot/pivotarea/only_data) | Indicates whether only the data values (in the data area of the view) for an item
| [only_label](/cells/python-net/aspose.cells.pivot/pivotarea/only_label) | Indicates whether only the data labels for an item selection are selected. |
| [is_row_grand_included](/cells/python-net/aspose.cells.pivot/pivotarea/is_row_grand_included) | Indicates whether the row grand total is included. |
| [is_column_grand_included](/cells/python-net/aspose.cells.pivot/pivotarea/is_column_grand_included) | Indicates whether the column grand total is included. |
| [axis_type](/cells/python-net/aspose.cells.pivot/pivotarea/axis_type) | Gets and sets the region of the PivotTable to which this rule applies. |
| [rule_type](/cells/python-net/aspose.cells.pivot/pivotarea/rule_type) | Gets and sets the type of selection rule. |
| [is_outline](/cells/python-net/aspose.cells.pivot/pivotarea/is_outline) | Indicates whether the rule refers to an area that is in outline mode. |
### Methods
| Method | Description |
| :- | :- |
| [`select_field(self, axis_type, field_name)`](/cells/python-net/aspose.cells.pivot/pivotarea/select_field/#aspose.cells.pivot.pivotfieldtype-system.string) | Select a field in the region as an area. |
| [`select_field(self, axis_type, field)`](/cells/python-net/aspose.cells.pivot/pivotarea/select_field/#aspose.cells.pivot.pivotfieldtype-aspose.cells.pivot.pivotfield) | Select a field in the region as an area. |
| [`select(self, axis_type, field_position, selection_type)`](/cells/python-net/aspose.cells.pivot/pivotarea/select/#aspose.cells.pivot.pivotfieldtype-int-aspose.cells.pivot.pivottableselectiontype) | Select the area with filters. |
| [`get_cell_areas(self)`](/cells/python-net/aspose.cells.pivot/pivotarea/get_cell_areas/#) | Gets cell areas of this pivot area. |
### See Also
* module [`aspose.cells.pivot`](..)
