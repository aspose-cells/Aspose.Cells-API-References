##Aspose::Cells::CellArea class
'Aspose::Cells::CellArea class. Represent an area of cells in C++.'
## CellArea class
Represent an area of cells.
```cpp
class CellArea
```
## Methods
| Method | Description |
| --- | --- |
| [CellArea()](./cellarea/) | Default constructor. |
| [CellArea(CellArea_Impl* impl)](./cellarea/) | Constructs from an implementation object. Internal use. |
| static [CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)](./createcellarea/) | Creates a cell area. |
| static [CreateCellArea(const U16String\& startCellName, const U16String\& endCellName)](./createcellarea/) | Creates a cell area. |
| static [CreateCellArea(const char16_t* startCellName, const char16_t* endCellName)](./createcellarea/) | Creates a cell area. |
| [ToString()](./tostring/) | Returns a string represents the current cell area object. |
## Fields
| Field | Description |
| --- | --- |
| [EndColumn](./endcolumn/) | Gets or set the end column of this area. |
| [EndRow](./endrow/) | Gets or set the end row of this area. |
| [StartColumn](./startcolumn/) | Gets or set the start column of this area. |
| [StartRow](./startrow/) | Gets or set the start row of this area. |
## Examples
```cpp
Aspose::Cells::Startup();
//Create Cell Area
CellArea ca;
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
