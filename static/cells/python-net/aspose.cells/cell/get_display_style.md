##get_display_style method
## get_display_style(self) {#}
Gets the display style of this cell.
### Returns
display style of this cell
```python
def get_display_style(self):
...
```
### Remarks
Same with using [`BorderType.SIDE_BORDERS`](/cells/python-net/aspose.cells/bordertype#SIDE_BORDERS)
for [`Cell.get_display_style`](/cells/python-net/aspose.cells/cell/get_display_style).
That is, this method will check and adjust top/bottom/left/right borders of this cell
according to the style([`Cell.get_style`](/cells/python-net/aspose.cells/cell/get_style)) of its adjacent cells,
but do not check the merged cells, and do not check the display style of adjacent cells.
## get_display_style(self, include_merged_borders) {#bool}
Gets the display style of this cell.
### Returns
display style of this cell
```python
def get_display_style(self, include_merged_borders):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| include_merged_borders | bool | Indicates whether checking borders of merged cells. |
### Remarks
If the specified flag is false, then it is same with [`Cell.get_display_style`](/cells/python-net/aspose.cells/cell/get_display_style).
Otherwise it is same with using
[`BorderType.SIDE_BORDERS`](/cells/python-net/aspose.cells/bordertype#SIDE_BORDERS)|[`BorderType.DYNAMIC_STYLE_BORDERS`](/cells/python-net/aspose.cells/bordertype#DYNAMIC_STYLE_BORDERS)
for [`Cell.get_display_style`](/cells/python-net/aspose.cells/cell/get_display_style).
## get_display_style(self, adjacent_borders) {#aspose.cells.BorderType}
Gets the display style of this cell.
### Returns
display style of this cell
```python
def get_display_style(self, adjacent_borders):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| adjacent_borders | aspose.cells.BorderType | Indicates which borders need to be checked and adjusted
### Remarks
If this cell is also affected by other settings such as conditional formatting, list objects, etc.,
then the display style may be different from [`Cell.get_style`](/cells/python-net/aspose.cells/cell/get_style).
For flags of adjusting borders according to adjacent cells,
[`BorderType.TOP_BORDER`](/cells/python-net/aspose.cells/bordertype#TOP_BORDER)/[`BorderType.BOTTOM_BORDER`](/cells/python-net/aspose.cells/bordertype#BOTTOM_BORDER)
/[`BorderType.LEFT_BORDER`](/cells/python-net/aspose.cells/bordertype#LEFT_BORDER)/[`BorderType.RIGHT_BORDER`](/cells/python-net/aspose.cells/bordertype#RIGHT_BORDER)
denote whether check and combine the bottom/top/right/left borders of
the left/right/top/bottom cells adjacent to this one.
For performance and compatibility consideration,
some enums are used to denote some special operations:
[`BorderType.HORIZONTAL`](/cells/python-net/aspose.cells/bordertype#HORIZONTAL)/[`BorderType.VERTICAL`](/cells/python-net/aspose.cells/bordertype#VERTICAL)
denote whether check and combine the bottom/right border of merged cells to this one.
[`BorderType.DIAGONAL`](/cells/python-net/aspose.cells/bordertype#DIAGONAL)(that is, both [`StyleModifyFlag.DIAGONAL_UP_BORDER`](/cells/python-net/aspose.cells/stylemodifyflag#DIAGONAL_UP_BORDER) and
[`StyleModifyFlag.DIAGONAL_DOWN_BORDER`](/cells/python-net/aspose.cells/stylemodifyflag#DIAGONAL_DOWN_BORDER) have been set) denotes check and combine borders
from the display style of adjacent cells.
Please note, checking borders/styles of adjacent cells, especially the display styles,
is time-consumed process. If there is no need to get the borders for the returned style,
using [`BorderType.NONE`](/cells/python-net/aspose.cells/bordertype#NONE) to disable the process of adjacent cells
will give better performance.
When getting borders of adjacent cells from styles defined on those cells only(without setting
[`BorderType.DIAGONAL`](/cells/python-net/aspose.cells/bordertype#DIAGONAL)), the performance also may be better because checking
the display style of one cell is time-consumed too.
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
* class [`Style`](/cells/python-net/aspose.cells/style)
