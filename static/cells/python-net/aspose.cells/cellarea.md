##CellArea class
## CellArea class
Represent an area of cells.
The CellArea type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/cellarea/__init__/#) | Constructs a new instance of CellArea |
### Properties
| Property | Description |
| :- | :- |
| [start_row](/cells/python-net/aspose.cells/cellarea/start_row) | Gets or set the start row of this area. |
| [end_row](/cells/python-net/aspose.cells/cellarea/end_row) | Gets or set the end row of this area. |
| [start_column](/cells/python-net/aspose.cells/cellarea/start_column) | Gets or set the start column of this area. |
| [end_column](/cells/python-net/aspose.cells/cellarea/end_column) | Gets or set the end column of this area. |
### Methods
| Method | Description |
| :- | :- |
| [`create_cell_area(, start_row, start_column, end_row, end_column)`](/cells/python-net/aspose.cells/cellarea/create_cell_area/#int-int-int-int) | Creates a cell area. |
| [`create_cell_area(, start_cell_name, end_cell_name)`](/cells/python-net/aspose.cells/cellarea/create_cell_area/#system.string-system.string) | Creates a cell area. |
| [`compare_to(self, obj)`](/cells/python-net/aspose.cells/cellarea/compare_to/#system.object) | Compare two CellArea objects according to their top-left corner. |
### Example
```python
from aspose.cells import CellArea
# Create Cell Area
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
```
### See Also
* module [`aspose.cells`](..)
