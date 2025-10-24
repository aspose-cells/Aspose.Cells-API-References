##Aspose::Cells::Cell::GetDisplayStyle method
'Aspose::Cells::Cell::GetDisplayStyle method. Gets the display style of this cell in C++.'
## Cell::GetDisplayStyle() method
Gets the display style of this cell.
```cpp
Style Aspose::Cells::Cell::GetDisplayStyle()
```
## ReturnValue
display style of this cell
## Remarks
Same with using [BorderType.SideBorders](../../bordertype/) for [GetDisplayStyle(BorderType)](./). That is, this method will check and adjust top/bottom/left/right borders of this cell according to the style([GetStyle()](../getstyle/)) of its adjacent cells, but do not check the merged cells, and do not check the display style of adjacent cells.
## See Also
* Class [Style](../../style/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::GetDisplayStyle(bool) method
Gets the display style of this cell.
```cpp
Style Aspose::Cells::Cell::GetDisplayStyle(bool includeMergedBorders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| includeMergedBorders | bool | Indicates whether checking borders of merged cells. |
## ReturnValue
display style of this cell
## Remarks
If the specified flag is false, then it is same with [GetDisplayStyle()](./). Otherwise it is same with using [BorderType.SideBorders](../../bordertype/)|[BorderType.DynamicStyleBorders](../../bordertype/) for [GetDisplayStyle(BorderType)](./).
## See Also
* Class [Style](../../style/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::GetDisplayStyle(BorderType) method
Gets the display style of this cell.
```cpp
Style Aspose::Cells::Cell::GetDisplayStyle(BorderType adjacentBorders)
```
| Parameter | Type | Description |
| --- | --- | --- |
| adjacentBorders | BorderType | Indicates which borders need to be checked and adjusted according to the borders of adjacent cells. |
## ReturnValue
display style of this cell
## Remarks
If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from [GetStyle()](../getstyle/).
For flags of adjusting borders according to adjacent cells, [BorderType.TopBorder](../../bordertype/)/[BorderType.BottomBorder](../../bordertype/)[BorderType.LeftBorder](../../bordertype/)/[BorderType.RightBorder](../../bordertype/) denote whether check and combine the bottom/top/right/left borders of the left/right/top/bottom cells adjacent to this one.
For performance and compatibility consideration, some enums are used to denote some special operations:
[BorderType.Horizontal](../../bordertype/)/[BorderType.Vertical](../../bordertype/) denote whether check and combine the bottom/right border of merged cells to this one.
[BorderType.Diagonal](../../bordertype/)(that is, both [StyleModifyFlag.DiagonalUpBorder](../../stylemodifyflag/) and [StyleModifyFlag.DiagonalDownBorder](../../stylemodifyflag/) have been set) denotes check and combine borders from the display style of adjacent cells.
Please note, checking borders/styles of adjacent cells, especially the display styles, is time-consumed process. If there is no need to get the borders for the returned style, using [BorderType.None](../../bordertype/) to disable the process of adjacent cells will give better performance. When getting borders of adjacent cells from styles defined on those cells only(without setting [BorderType.Diagonal](../../bordertype/)), the performance also may be better because checking the display style of one cell is time-consumed too.
## See Also
* Class [Style](../../style/)
* Enum [BorderType](../../bordertype/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
