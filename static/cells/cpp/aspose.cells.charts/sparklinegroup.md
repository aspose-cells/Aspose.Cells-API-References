##Aspose::Cells::Charts::SparklineGroup class
'Aspose::Cells::Charts::SparklineGroup class. Sparkline is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines in C++.'
## SparklineGroup class
[Sparkline](../sparkline/) is organized into sparkline group. A [SparklineGroup](./) contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.
```cpp
class SparklineGroup
```
## Methods
| Method | Description |
| --- | --- |
| [GetDisplayHidden()](./getdisplayhidden/) | Indicates whether to show data in hidden rows and columns. |
| [GetFirstPointColor()](./getfirstpointcolor/) | Gets and sets the color of the first point of data in the sparkline group. |
| [GetHighPointColor()](./gethighpointcolor/) | Gets and sets the color of the highest points of data in the sparkline group. |
| [GetHorizontalAxisColor()](./gethorizontalaxiscolor/) | Gets and sets the color of the horizontal axis in the sparkline group. |
| [GetHorizontalAxisDateRange()](./gethorizontalaxisdaterange/) | Represents the range that contains the date values for the sparkline data. |
| [GetLastPointColor()](./getlastpointcolor/) | Gets and sets the color of the last point of data in the sparkline group. |
| [GetLineWeight()](./getlineweight/) | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [GetLowPointColor()](./getlowpointcolor/) | Gets and sets the color of the lowest points of data in the sparkline group. |
| [GetMarkersColor()](./getmarkerscolor/) | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [GetNegativePointsColor()](./getnegativepointscolor/) | Gets and sets the color of the negative values on the sparkline group. |
| [GetPlotEmptyCellsType()](./getplotemptycellstype/) | Indicates how to plot empty cells. |
| [GetPlotRightToLeft()](./getplotrighttoleft/) | Indicates whether the plot data is right to left. |
| [GetPresetStyle()](./getpresetstyle/) | Gets and sets the preset style type of the sparkline group. |
| [GetSeriesColor()](./getseriescolor/) | Gets and sets the color of the sparklines in the sparkline group. |
| [GetShowFirstPoint()](./getshowfirstpoint/) | Indicates whether to highlight the first point of data in the sparkline group. |
| [GetShowHighPoint()](./getshowhighpoint/) | Indicates whether to highlight the highest points of data in the sparkline group. |
| [GetShowHorizontalAxis()](./getshowhorizontalaxis/) | Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis. |
| [GetShowLastPoint()](./getshowlastpoint/) | Indicates whether to highlight the last point of data in the sparkline group. |
| [GetShowLowPoint()](./getshowlowpoint/) | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [GetShowMarkers()](./getshowmarkers/) | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [GetShowNegativePoints()](./getshownegativepoints/) | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [GetSparklines()](./getsparklines/) | Gets the collection of [Sparkline](../sparkline/) object. |
| [GetType()](./gettype/) | Indicates the sparkline type of the sparkline group. |
| [GetVerticalAxisMaxValue()](./getverticalaxismaxvalue/) | Gets and sets the custom maximum value for the vertical axis. |
| [GetVerticalAxisMaxValueType()](./getverticalaxismaxvaluetype/) | Represents the vertical axis maximum value type. |
| [GetVerticalAxisMinValue()](./getverticalaxisminvalue/) | Gets and sets the custom minimum value for the vertical axis. |
| [GetVerticalAxisMinValueType()](./getverticalaxisminvaluetype/) | Represents the vertical axis minimum value type. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SparklineGroup\& src)](./operator_asm/) | operator= |
| [ResetRanges(const U16String\& dataRange, bool isVertical, const CellArea\& locationRange)](./resetranges/) | Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges. |
| [ResetRanges(const char16_t* dataRange, bool isVertical, const CellArea\& locationRange)](./resetranges/) | Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges. |
| [SetDisplayHidden(bool value)](./setdisplayhidden/) | Indicates whether to show data in hidden rows and columns. |
| [SetFirstPointColor(const CellsColor\& value)](./setfirstpointcolor/) | Gets and sets the color of the first point of data in the sparkline group. |
| [SetHighPointColor(const CellsColor\& value)](./sethighpointcolor/) | Gets and sets the color of the highest points of data in the sparkline group. |
| [SetHorizontalAxisColor(const CellsColor\& value)](./sethorizontalaxiscolor/) | Gets and sets the color of the horizontal axis in the sparkline group. |
| [SetHorizontalAxisDateRange(const U16String\& value)](./sethorizontalaxisdaterange/) | Represents the range that contains the date values for the sparkline data. |
| [SetHorizontalAxisDateRange(const char16_t* value)](./sethorizontalaxisdaterange/) | Represents the range that contains the date values for the sparkline data. |
| [SetLastPointColor(const CellsColor\& value)](./setlastpointcolor/) | Gets and sets the color of the last point of data in the sparkline group. |
| [SetLineWeight(double value)](./setlineweight/) | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [SetLowPointColor(const CellsColor\& value)](./setlowpointcolor/) | Gets and sets the color of the lowest points of data in the sparkline group. |
| [SetMarkersColor(const CellsColor\& value)](./setmarkerscolor/) | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [SetNegativePointsColor(const CellsColor\& value)](./setnegativepointscolor/) | Gets and sets the color of the negative values on the sparkline group. |
| [SetPlotEmptyCellsType(PlotEmptyCellsType value)](./setplotemptycellstype/) | Indicates how to plot empty cells. |
| [SetPlotRightToLeft(bool value)](./setplotrighttoleft/) | Indicates whether the plot data is right to left. |
| [SetPresetStyle(SparklinePresetStyleType value)](./setpresetstyle/) | Gets and sets the preset style type of the sparkline group. |
| [SetSeriesColor(const CellsColor\& value)](./setseriescolor/) | Gets and sets the color of the sparklines in the sparkline group. |
| [SetShowFirstPoint(bool value)](./setshowfirstpoint/) | Indicates whether to highlight the first point of data in the sparkline group. |
| [SetShowHighPoint(bool value)](./setshowhighpoint/) | Indicates whether to highlight the highest points of data in the sparkline group. |
| [SetShowHorizontalAxis(bool value)](./setshowhorizontalaxis/) | Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis. |
| [SetShowLastPoint(bool value)](./setshowlastpoint/) | Indicates whether to highlight the last point of data in the sparkline group. |
| [SetShowLowPoint(bool value)](./setshowlowpoint/) | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [SetShowMarkers(bool value)](./setshowmarkers/) | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [SetShowNegativePoints(bool value)](./setshownegativepoints/) | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [SetType(SparklineType value)](./settype/) | Indicates the sparkline type of the sparkline group. |
| [SetVerticalAxisMaxValue(double value)](./setverticalaxismaxvalue/) | Gets and sets the custom maximum value for the vertical axis. |
| [SetVerticalAxisMaxValueType(SparklineAxisMinMaxType value)](./setverticalaxismaxvaluetype/) | Represents the vertical axis maximum value type. |
| [SetVerticalAxisMinValue(double value)](./setverticalaxisminvalue/) | Gets and sets the custom minimum value for the vertical axis. |
| [SetVerticalAxisMinValueType(SparklineAxisMinMaxType value)](./setverticalaxisminvaluetype/) | Represents the vertical axis minimum value type. |
| [SparklineGroup(SparklineGroup_Impl* impl)](./sparklinegroup/) | Constructs from an implementation object. |
| [SparklineGroup(const SparklineGroup\& src)](./sparklinegroup/) | Copy constructor. |
| [~SparklineGroup()](./~sparklinegroup/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook book;
Worksheet sheet = book.GetWorksheets().Get(0);
sheet.GetCells().Get(u"A1").PutValue(5);
sheet.GetCells().Get(u"B1").PutValue(2);
sheet.GetCells().Get(u"C1").PutValue(1);
sheet.GetCells().Get(u"D1").PutValue(3);
// Define the CellArea
CellArea ca;
ca.StartColumn = 4;
ca.EndColumn = 4;
ca.StartRow = 0;
ca.EndRow = 0;
int idx = sheet.GetSparklineGroups().Add(SparklineType::Line, u"A1:D1", false, ca);
SparklineGroup group = sheet.GetSparklineGroups().Get(idx);
group.GetSparklines().Add(sheet.GetName() + u"!A1:D1", 0, 4);
// Create CellsColor
CellsColor clr = book.CreateCellsColor();
clr.SetColor(Color{ 0xff, 0xff, 0xa5, 0 });//Orange
group.SetSeriesColor(clr);
// set the high points are colored green and the low points are colored red
group.SetShowHighPoint(true);
group.SetShowLowPoint(true);
group.GetHighPointColor().SetColor(Color{0xff, 0, 0x80, 0});//Green
group.GetLowPointColor().SetColor(Color{0xff, 0xff, 0, 0});//Red
// set line weight
group.SetLineWeight(1.0);
book.Save(u"output.xlsx", SaveFormat::Xlsx);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
