---
title: Cell.GetDisplayStyle
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the display style of this cell
type: docs
url: /net/aspose.cells/cell/getdisplaystyle/
---
## GetDisplayStyle() {#getdisplaystyle}

Gets the display style of this cell.

```csharp
public Style GetDisplayStyle()
```

### Return Value

display style of this cell

### Remarks

Same with using SideBorders for `GetDisplayStyle`. That is, this method will check and adjust top/bottom/left/right borders of this cell according to the style([`GetStyle`](../getstyle/)) of its adjacent cells, but do not check the merged cells, and do not check the display style of adjacent cells.

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(bool) {#getdisplaystyle_2}

Gets the display style of this cell.

```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| includeMergedBorders | Boolean | Indicates whether checking borders of merged cells. |

### Return Value

display style of this cell

### Remarks

If the specified flag is false, then it is same with `GetDisplayStyle`. Otherwise it is same with using SideBorders&#x7C;DynamicStyleBorders for `GetDisplayStyle`.

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(BorderType) {#getdisplaystyle_1}

Gets the display style of this cell.

```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| adjacentBorders | BorderType | Indicates which borders need to be checked and adjusted according to the borders of adjacent cells. |

### Return Value

display style of this cell

### Remarks

If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from [`GetStyle`](../getstyle/). For flags of adjusting borders according to adjacent cells, TopBorder/BottomBorder /LeftBorder/RightBorder denote whether check and combine the bottom/top/right/left borders of the left/right/top/bottom cells adjacent to this one. For performance and compatibility consideration, some enums are used to denote some special operations: Horizontal/Vertical denote whether check and combine the bottom/right border of merged cells to this one. Diagonal(that is, both DiagonalUpBorder and DiagonalDownBorder have been set) denotes check and combine borders from the display style of adjacent cells. Please note, checking borders/styles of adjacent cells, especially the display styles, is time-consumed process. If there is no need to get the borders for the returned style, using None to disable the process of adjacent cells will give better performance. When getting borders of adjacent cells from styles defined on those cells only(without setting Diagonal), the performance also may be better because checking the display style of one cell is time-consumed too.

### See Also

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


