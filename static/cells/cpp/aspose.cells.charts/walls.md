##Aspose::Cells::Charts::Walls class
'Aspose::Cells::Charts::Walls class. Encapsulates the object that represents the walls of a 3-D chart in C++.'
## Walls class
Encapsulates the object that represents the walls of a 3-D chart.
```cpp
class Walls : public Aspose::Cells::Charts::Floor
```
## Methods
| Method | Description |
| --- | --- |
| [Area(Area_Impl* impl)](../../aspose.cells.drawing/area/area/) | Constructs from an implementation object. |
| [Area(const Area\& src)](../../aspose.cells.drawing/area/area/) | Copy constructor. |
| [Floor(Floor_Impl* impl)](../floor/floor/) | Constructs from an implementation object. |
| [Floor(const Floor\& src)](../floor/floor/) | Copy constructor. |
| [Floor(const Area\& src)](../floor/floor/) | Constructs from a parent object. |
| [GetBackgroundColor()](../../aspose.cells.drawing/area/getbackgroundcolor/) | Gets or sets the background [Color](../../aspose.cells/color/) of the [Area](../../aspose.cells.drawing/area/). |
| [GetBorder()](../floor/getborder/) | Gets or sets the border Line. |
| [GetCenterX()](./getcenterx/) | Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetCenterXPx()](./getcenterxpx/) | Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetCenterY()](./getcentery/) | Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetCenterYPx()](./getcenterypx/) | Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetCubePointCount()](./getcubepointcount/) | Gets the number of cube points after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetCubePointXPx(int32_t index)](./getcubepointxpx/) | Gets x-coordinate of the apex point of walls cube after calls [Chart.Calculate()](../chart/calculate/) method. The number of apex points of walls cube is eight. |
| [GetCubePointYPx(int32_t index)](./getcubepointypx/) | Gets y-coordinate of the apex point of walls cube after calls [Chart.Calculate()](../chart/calculate/) method. The number of apex points of walls cube is eight. |
| [GetDepth()](./getdepth/) | Gets the depth front to back in units of 1/4000 of chart's width after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetDepthPx()](./getdepthpx/) | Gets the depth front to back in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetFillFormat()](../../aspose.cells.drawing/area/getfillformat/) | Represents a [FillFormat](../../aspose.cells.drawing/fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [GetForegroundColor()](../../aspose.cells.drawing/area/getforegroundcolor/) | Gets or sets the foreground [Color](../../aspose.cells/color/). |
| [GetFormatting()](../../aspose.cells.drawing/area/getformatting/) | Represents the formatting of the area. |
| [GetHeight()](./getheight/) | Gets the height of top to bottom in units of 1/4000 of chart's height after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetHeightPx()](./getheightpx/) | Gets the height of top to bottom in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetInvertIfNegative()](../../aspose.cells.drawing/area/getinvertifnegative/) | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [GetTransparency()](../../aspose.cells.drawing/area/gettransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [GetWidth()](./getwidth/) | Gets the width of left to right in units of 1/4000 of chart's width after calls [Chart.Calculate()](../chart/calculate/) method. |
| [GetWidthPx()](./getwidthpx/) | Gets the width of left to right in units of pixels after calls [Chart.Calculate()](../chart/calculate/) method. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Walls\& src)](./operator_asm/) | operator= |
| [operator=(const Floor\& src)](../floor/operator_asm/) | operator= |
| [operator=(const Area\& src)](../../aspose.cells.drawing/area/operator_asm/) | operator= |
| [SetBackgroundColor(const Aspose::Cells::Color\& value)](../../aspose.cells.drawing/area/setbackgroundcolor/) | Gets or sets the background [Color](../../aspose.cells/color/) of the [Area](../../aspose.cells.drawing/area/). |
| [SetBorder(const Line\& value)](../floor/setborder/) | Gets or sets the border Line. |
| [SetForegroundColor(const Aspose::Cells::Color\& value)](../../aspose.cells.drawing/area/setforegroundcolor/) | Gets or sets the foreground [Color](../../aspose.cells/color/). |
| [SetFormatting(FormattingType value)](../../aspose.cells.drawing/area/setformatting/) | Represents the formatting of the area. |
| [SetInvertIfNegative(bool value)](../../aspose.cells.drawing/area/setinvertifnegative/) | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [SetTransparency(double value)](../../aspose.cells.drawing/area/settransparency/) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [Walls(Walls_Impl* impl)](./walls/) | Constructs from an implementation object. |
| [Walls(const Walls\& src)](./walls/) | Copy constructor. |
| [Walls(const Floor\& src)](./walls/) | Constructs from a parent object. |
| [~Area()](../../aspose.cells.drawing/area/~area/) | Destructor. |
| [~Floor()](../floor/~floor/) | Destructor. |
| [~Walls()](./~walls/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [Floor](../floor/)
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
