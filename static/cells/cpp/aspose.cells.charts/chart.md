##Aspose::Cells::Charts::Chart class
'Aspose::Cells::Charts::Chart class. Encapsulates the object that represents a single Excel chart in C++.'
## Chart class
Encapsulates the object that represents a single Excel chart.
```cpp
class Chart
```
## Methods
| Method | Description |
| --- | --- |
| [Calculate()](./calculate/) | Calculates the custom position of plot area, axes if the position of them are auto assigned. |
| [Calculate(const ChartCalculateOptions\& calculateOptions)](./calculate/) | Calculates the custom position of plot area, axes if the position of them are auto assigned, with [Chart](./) Calculate Options. |
| [ChangeTemplate(const Vector \<uint8_t\>\& data)](./changetemplate/) | Change chart type with preset template. |
| [Chart(Chart_Impl* impl)](./chart/) | Constructs from an implementation object. |
| [Chart(const Chart\& src)](./chart/) | Copy constructor. |
| [GetActualSize()](./getactualsize/) | Gets actual size of chart in unit of pixels. |
| [GetAutoScaling()](./getautoscaling/) | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True. |
| [GetBackWall()](./getbackwall/) | Returns a [Walls](../walls/) object that represents the back wall of a 3-D chart. |
| [GetCategoryAxis()](./getcategoryaxis/) | Gets the chart's X axis. |
| [GetChartArea()](./getchartarea/) | Gets the chart area in the worksheet. |
| [GetChartDataRange()](./getchartdatarange/) | Gets the data source range of the chart. |
| [GetChartDataTable()](./getchartdatatable/) | Represents the chart data table. |
| [GetChartObject()](./getchartobject/) | Represents the chartShape;. |
| [GetDepthPercent()](./getdepthpercent/) | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [GetDisplayNaAsBlank()](./getdisplaynaasblank/) | Indicates whether displaying #N/A as blank value. |
| [GetElevation()](./getelevation/) | Represents the elevation of the 3-D chart view, in degrees. |
| [GetFilteredNSeries()](./getfilterednseries/) | Gets a [SeriesCollection](../seriescollection/) collection representing the data series that are filtered in the chart. |
| [GetFirstSliceAngle()](./getfirstsliceangle/) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [GetFloor()](./getfloor/) | Returns a [Floor](../floor/) object that represents the walls of a 3-D chart. |
| [GetGapDepth()](./getgapdepth/) | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500. |
| [GetGapWidth()](./getgapwidth/) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [GetHeightPercent()](./getheightpercent/) | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [GetHidePivotFieldButtons()](./gethidepivotfieldbuttons/) | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [GetIs3D()](./getis3d/) | Indicates whether the chart is a 3d chart. |
| [GetLegend()](./getlegend/) | Gets the chart legend. |
| [GetLine()](./getline/) | Gets the line. |
| [GetName()](./getname/) | Gets and sets the name of the chart. |
| [GetNSeries()](./getnseries/) | Gets a [SeriesCollection](../seriescollection/) collection representing the data series in the chart. |
| [GetPageSetup()](./getpagesetup/) | Represents the page setup description in this chart. |
| [GetPerspective()](./getperspective/) | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True. |
| [GetPivotOptions()](./getpivotoptions/) | Specifies the pivot controls that appear on the chart. |
| [GetPivotSource()](./getpivotsource/) | The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. |
| [GetPlacement()](./getplacement/) | Represents the way the chart is attached to the cells below it. |
| [GetPlotArea()](./getplotarea/) | Gets the chart's plot area which includes axis tick labels. |
| [GetPlotBy()](./getplotby/) | Gets and sets whether plot by row or column. |
| [GetPlotEmptyCellsType()](./getplotemptycellstype/) | Gets and sets how to plot the empty cells. |
| [GetPlotVisibleCellsOnly()](./getplotvisiblecellsonly/) | Indicates whether plot visible cells only. |
| [GetPrintSize()](./getprintsize/) | Gets and sets the printed chart size. |
| [GetRightAngleAxes()](./getrightangleaxes/) | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie [Charts](../)). |
| [GetRotationAngle()](./getrotationangle/) | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
| [GetSecondCategoryAxis()](./getsecondcategoryaxis/) | Gets the chart's second X axis. |
| [GetSecondValueAxis()](./getsecondvalueaxis/) | Gets the chart's second Y axis. |
| [GetSeriesAxis()](./getseriesaxis/) | Gets the chart's series axis. |
| [GetShapes()](./getshapes/) | Returns all drawing shapes in this chart. |
| [GetShowDataTable()](./getshowdatatable/) | Gets or sets a value indicating whether the chart displays a data table. |
| [GetShowLegend()](./getshowlegend/) | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [GetSideWall()](./getsidewall/) | Returns a [Walls](../walls/) object that represents the side wall of a 3-D chart. |
| [GetSizeWithWindow()](./getsizewithwindow/) | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [GetStyle()](./getstyle/) | Gets and sets the builtin style. |
| [GetSubTitle()](./getsubtitle/) | Gets the chart's sub-title. Only for ODS format file. |
| [GetTitle()](./gettitle/) | Gets the chart's title. |
| [GetType()](./gettype/) | Gets or sets a chart's type. |
| [GetValueAxis()](./getvalueaxis/) | Gets the chart's Y axis. |
| [GetWalls()](./getwalls/) | Returns a [Walls](../walls/) object that represents the walls of a 3-D chart. |
| [GetWallsAndGridlines2D()](./getwallsandgridlines2d/) | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [GetWorksheet()](./getworksheet/) | Gets the worksheet which contains this chart. |
| [HasAxis(AxisType aixsType, bool isPrimary)](./hasaxis/) | Returns which axes exist on the chart. |
| [IsCellReferedByChart(int32_t sheetIndex, int32_t rowIndex, int32_t columnIndex)](./iscellreferedbychart/) | Returns whether the cell refered by the chart. |
| [IsChartDataChanged()](./ischartdatachanged/) | Detects if a chart's data source has changed. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsRectangularCornered()](./isrectangularcornered/) | Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true. |
| [Move(int32_t upperLeftRow, int32_t upperLeftColumn, int32_t lowerRightRow, int32_t lowerRightColumn)](./move/) | Moves the chart to a specified location. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Chart\& src)](./operator_asm/) | operator= |
| [RefreshPivotData()](./refreshpivotdata/) | Refreshes chart's data from pivot table. |
| [SetAutoScaling(bool value)](./setautoscaling/) | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True. |
| [SetChartDataRange(const U16String\& area, bool isVertical)](./setchartdatarange/) | Specifies data range for a chart. |
| [SetChartDataRange(const char16_t* area, bool isVertical)](./setchartdatarange/) | Specifies data range for a chart. |
| [SetDepthPercent(int32_t value)](./setdepthpercent/) | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [SetDisplayNaAsBlank(bool value)](./setdisplaynaasblank/) | Indicates whether displaying #N/A as blank value. |
| [SetElevation(int32_t value)](./setelevation/) | Represents the elevation of the 3-D chart view, in degrees. |
| [SetFirstSliceAngle(int32_t value)](./setfirstsliceangle/) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [SetGapDepth(int32_t value)](./setgapdepth/) | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500. |
| [SetGapWidth(int32_t value)](./setgapwidth/) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [SetHeightPercent(int32_t value)](./setheightpercent/) | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [SetHidePivotFieldButtons(bool value)](./sethidepivotfieldbuttons/) | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [SetIsRectangularCornered(bool value)](./setisrectangularcornered/) | Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true. |
| [SetName(const U16String\& value)](./setname/) | Gets and sets the name of the chart. |
| [SetName(const char16_t* value)](./setname/) | Gets and sets the name of the chart. |
| [SetPerspective(int16_t value)](./setperspective/) | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True. |
| [SetPivotSource(const U16String\& value)](./setpivotsource/) | The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. |
| [SetPivotSource(const char16_t* value)](./setpivotsource/) | The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. |
| [SetPlacement(PlacementType value)](./setplacement/) | Represents the way the chart is attached to the cells below it. |
| [SetPlotEmptyCellsType(PlotEmptyCellsType value)](./setplotemptycellstype/) | Gets and sets how to plot the empty cells. |
| [SetPlotVisibleCellsOnly(bool value)](./setplotvisiblecellsonly/) | Indicates whether plot visible cells only. |
| [SetPrintSize(PrintSizeType value)](./setprintsize/) | Gets and sets the printed chart size. |
| [SetRightAngleAxes(bool value)](./setrightangleaxes/) | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie [Charts](../)). |
| [SetRotationAngle(int32_t value)](./setrotationangle/) | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
| [SetShowDataTable(bool value)](./setshowdatatable/) | Gets or sets a value indicating whether the chart displays a data table. |
| [SetShowLegend(bool value)](./setshowlegend/) | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [SetSizeWithWindow(bool value)](./setsizewithwindow/) | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [SetStyle(int32_t value)](./setstyle/) | Gets and sets the builtin style. |
| [SetType(ChartType value)](./settype/) | Gets or sets a chart's type. |
| [SetWallsAndGridlines2D(bool value)](./setwallsandgridlines2d/) | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [SwitchRowColumn()](./switchrowcolumn/) | Switches row/column. |
| [ToImage(const U16String\& imageFile)](./toimage/) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [ToImage(const char16_t* imageFile)](./toimage/) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [ToImage(const U16String\& imageFile, Aspose::Cells::Drawing::ImageType imageType)](./toimage/) | Creates the chart image and saves it to a file in the specified image type. |
| [ToImage(const char16_t* imageFile, Aspose::Cells::Drawing::ImageType imageType)](./toimage/) | Creates the chart image and saves it to a file in the specified image type. |
| [ToImage(const U16String\& imageFile, int64_t jpegQuality)](./toimage/) |  **(Deprecated)** Creates the chart image and saves it to a file in the Jpeg format. |
| [ToImage(const char16_t* imageFile, int64_t jpegQuality)](./toimage/) |  **(Deprecated)** Creates the chart image and saves it to a file in the Jpeg format. |
| [ToImage(int64_t jpegQuality)](./toimage/) | Creates the chart image and saves it to a stream in the Jpeg format. |
| [ToImage(Aspose::Cells::Drawing::ImageType imageType)](./toimage/) | Creates the chart image and saves it to a stream in the specified format. |
| [ToImage(const U16String\& imageFile, const ImageOrPrintOptions\& options)](./toimage/) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [ToImage(const char16_t* imageFile, const ImageOrPrintOptions\& options)](./toimage/) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [ToImage(const ImageOrPrintOptions\& options)](./toimage/) | Creates the chart image and saves it to a stream in the specified format. |
| [ToPdf(const U16String\& fileName)](./topdf/) | Saves the chart to a pdf file. |
| [ToPdf(const char16_t* fileName)](./topdf/) | Saves the chart to a pdf file. |
| [ToPdf(const U16String\& fileName, float desiredPageWidth, float desiredPageHeight, PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)](./topdf/) | Saves the chart to a pdf file. |
| [ToPdf(const char16_t* fileName, float desiredPageWidth, float desiredPageHeight, PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)](./topdf/) | Saves the chart to a pdf file. |
| [ToPdf()](./topdf/) | Creates the chart pdf and saves it to a stream. |
| [ToPdf(float desiredPageWidth, float desiredPageHeight, PageLayoutAlignmentType hAlignmentType, PageLayoutAlignmentType vAlignmentType)](./topdf/) | Creates the chart pdf and saves it to a stream. |
| [~Chart()](./~chart/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//The following codes show how to create a chart with c++ codes.
Workbook workbook;
Worksheet sheet = workbook.GetWorksheets().Get(0);
Cells cells = sheet.GetCells();
cells.Get(0, 1).PutValue(u"Income");
cells.Get(1, 0).PutValue(u"Company A");
cells.Get(2, 0).PutValue(u"Company B");
cells.Get(3, 0).PutValue(u"Company C");
cells.Get(1, 1).PutValue(10000);
cells.Get(2, 1).PutValue(20000);
cells.Get(3, 1).PutValue(30000);
int chartIndex = sheet.GetCharts().Add(ChartType::Column, 9, 9, 21, 15);
Chart chart = sheet.GetCharts().Get(chartIndex);
chart.SetChartDataRange(u"A1:B4", true);
chart.SetShowLegend(true);
chart.GetTitle().SetText(u"Income Analysis");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
