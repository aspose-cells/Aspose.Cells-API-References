##Chart Class
'Chart class. Encapsulates the object that represents chart in Go.'
## Chart class
Encapsulates the object that represents a single Excel chart.
```go
type Chart struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetStyle](./getstyle/) | Gets and sets the builtin style. |
|[SetStyle](./setstyle/) | Gets and sets the builtin style. |
|[GetChartObject](./getchartobject/) | Represents the chartShape; |
|[GetHidePivotFieldButtons](./gethidepivotfieldbuttons/) | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
|[SetHidePivotFieldButtons](./sethidepivotfieldbuttons/) | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
|[GetPivotOptions](./getpivotoptions/) | Specifies the pivot controls that appear on the chart |
|[GetPivotSource](./getpivotsource/) | The source is the data of the pivotTable.If PivotSource is not empty ,the chart is PivotChart. |
|[SetPivotSource](./setpivotsource/) | The source is the data of the pivotTable.If PivotSource is not empty ,the chart is PivotChart. |
|[IsCellReferedByChart](./iscellreferedbychart/) | Returns whether the cell refered by the chart. |
|[IsChartDataChanged](./ischartdatachanged/) | Detects if a chart's data source has changed. |
|[GetPlotBy](./getplotby/) | Gets and sets whether plot by row or column. |
|[RefreshPivotData](./refreshpivotdata/) | Refreshes chart's data from pivot table. |
|[GetPlotEmptyCellsType](./getplotemptycellstype/) | Gets and sets  how to plot the empty cells. |
|[SetPlotEmptyCellsType](./setplotemptycellstype/) | Gets and sets  how to plot the empty cells. |
|[GetPlotVisibleCellsOnly](./getplotvisiblecellsonly/) | Indicates whether plot visible cells only. |
|[SetPlotVisibleCellsOnly](./setplotvisiblecellsonly/) | Indicates whether plot visible cells only. |
|[GetDisplayNaAsBlank](./getdisplaynaasblank/) | Indicates whether displaying #N/A as blank value. |
|[SetDisplayNaAsBlank](./setdisplaynaasblank/) | Indicates whether displaying #N/A as blank value. |
|[GetName](./getname/) | Gets and sets the name of the chart. |
|[SetName](./setname/) | Gets and sets the name of the chart. |
|[GetSizeWithWindow](./getsizewithwindow/) | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
|[SetSizeWithWindow](./setsizewithwindow/) | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet which contains this chart. |
|[GetShapes](./getshapes/) | Returns all drawing shapes in this chart. |
|[GetPrintSize](./getprintsize/) | Gets and sets the printed chart size. |
|[SetPrintSize](./setprintsize/) | Gets and sets the printed chart size. |
|[ChangeTemplate](./changetemplate/) | Change chart type with preset template. |
|[GetType](./gettype/) | Gets or sets a chart's type. |
|[SetType](./settype/) | Gets or sets a chart's type. |
|[Move](./move/) | Moves the chart to a specified location. |
|[GetNSeries](./getnseries/) | Gets a SeriesCollection collection representing the data series in the chart. |
|[GetFilteredNSeries](./getfilterednseries/) | Gets a SeriesCollection collection representing the data series that are filtered in the chart. |
|[GetTitle](./gettitle/) | Gets the chart's title. |
|[GetSubTitle](./getsubtitle/) | Gets the chart's sub-title.Only for ODS format file. |
|[GetPlotArea](./getplotarea/) | Gets the chart's plot area which includes axis tick labels. |
|[GetChartArea](./getchartarea/) | Gets the chart area in the worksheet. |
|[GetCategoryAxis](./getcategoryaxis/) | Gets the chart's X axis. |
|[GetValueAxis](./getvalueaxis/) | Gets the chart's Y axis. |
|[GetSecondValueAxis](./getsecondvalueaxis/) | Gets the chart's second Y axis. |
|[GetSecondCategoryAxis](./getsecondcategoryaxis/) | Gets the chart's second X axis. |
|[GetSeriesAxis](./getseriesaxis/) | Gets the chart's series axis. |
|[GetLegend](./getlegend/) | Gets the chart legend. |
|[GetChartDataTable](./getchartdatatable/) | Represents the chart data table. |
|[GetShowLegend](./getshowlegend/) | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
|[SetShowLegend](./setshowlegend/) | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
|[IsRectangularCornered](./isrectangularcornered/) | Gets or sets a value indicating whether the chart area is rectangular cornered.Default is true. |
|[SetIsRectangularCornered](./setisrectangularcornered/) | Gets or sets a value indicating whether the chart area is rectangular cornered.Default is true. |
|[GetShowDataTable](./getshowdatatable/) | Gets or sets a value indicating whether the chart displays a data table. |
|[SetShowDataTable](./setshowdatatable/) | Gets or sets a value indicating whether the chart displays a data table. |
|[GetFirstSliceAngle](./getfirstsliceangle/) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical).Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
|[SetFirstSliceAngle](./setfirstsliceangle/) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical).Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
|[GetGapWidth](./getgapwidth/) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width.The value of this property must be between 0 and 500. |
|[SetGapWidth](./setgapwidth/) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width.The value of this property must be between 0 and 500. |
|[GetGapDepth](./getgapdepth/) | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width.The value of this property must be between 0 and 500. |
|[SetGapDepth](./setgapdepth/) | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width.The value of this property must be between 0 and 500. |
|[Calculate](./calculate/) | Calculates the custom position of plot area, axes if the position of them are auto assigned. |
|[Calculate_ChartCalculateOptions](./calculate_chartcalculateoptions/) | Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options. |
|[GetFloor](./getfloor/) | Returns a Floor object that represents the walls of a 3-D chart. |
|[GetWalls](./getwalls/) | Returns a Walls object that represents the walls of a 3-D chart. |
|[GetBackWall](./getbackwall/) | Returns a Walls object that represents the back wall of a 3-D chart. |
|[GetSideWall](./getsidewall/) | Returns a Walls object that represents the side wall of a 3-D chart. |
|[GetWallsAndGridlines2D](./getwallsandgridlines2d/) | True if gridlines are drawn two-dimensionally on a 3-D chart. |
|[SetWallsAndGridlines2D](./setwallsandgridlines2d/) | True if gridlines are drawn two-dimensionally on a 3-D chart. |
|[GetRotationAngle](./getrotationangle/) | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
|[SetRotationAngle](./setrotationangle/) | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
|[GetElevation](./getelevation/) | Represents the elevation of the 3-D chart view, in degrees. |
|[SetElevation](./setelevation/) | Represents the elevation of the 3-D chart view, in degrees. |
|[GetRightAngleAxes](./getrightangleaxes/) | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). |
|[SetRightAngleAxes](./setrightangleaxes/) | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). |
|[GetAutoScaling](./getautoscaling/) | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart.The RightAngleAxes property must be True. |
|[SetAutoScaling](./setautoscaling/) | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart.The RightAngleAxes property must be True. |
|[GetHeightPercent](./getheightpercent/) | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
|[SetHeightPercent](./setheightpercent/) | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
|[GetPerspective](./getperspective/) | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100.This property is ignored if the RightAngleAxes property is True. |
|[SetPerspective](./setperspective/) | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100.This property is ignored if the RightAngleAxes property is True. |
|[GetIs3D](./getis3d/) | Indicates whether the chart is a 3d chart. |
|[GetDepthPercent](./getdepthpercent/) | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
|[SetDepthPercent](./setdepthpercent/) | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
|[ToImage_String](./toimage_string/) | Creates the chart image and saves it to a file.The extension of the file name determines the format of the image. |
|[ToImage_String_ImageType](./toimage_string_imagetype/) | Creates the chart image and saves it to a file in the specified image type. |
|[ToImage_Int64](./toimage_int64/) | Creates the chart image and saves it to a stream in the Jpeg format. |
|[ToImage_ImageType](./toimage_imagetype/) | Creates the chart image and saves it to a stream in the specified format. |
|[ToPdf_String](./topdf_string/) | Saves the chart to a pdf file. |
|[ToPdf_String_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_string_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Saves the chart to a pdf file. |
|[ToPdf](./topdf/) | Creates the chart pdf and saves it to a stream. |
|[ToPdf_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | Creates the chart pdf and saves it to a stream. |
|[ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | Creates the chart image and saves it to a file.The extension of the file name determines the format of the image. |
|[ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | Creates the chart image and saves it to a stream in the specified format. |
|[GetActualSize](./getactualsize/) | Gets actual size of chart in unit of pixels. |
|[GetPlacement](./getplacement/) | Represents the way the chart is attached to the cells below it. |
|[SetPlacement](./setplacement/) | Represents the way the chart is attached to the cells below it. |
|[GetPageSetup](./getpagesetup/) | Represents the page setup description in this chart. |
|[HasAxis](./hasaxis/) | Returns which axes exist on the chart. |
|[SwitchRowColumn](./switchrowcolumn/) | Switches row/column. |
|[GetChartDataRange](./getchartdatarange/) | Gets the data source range of the chart. |
|[SetChartDataRange](./setchartdatarange/) | Specifies data range for a chart. |
|[GetLine](./getline/) | Gets the line. |
