##ChartType Enum
'ChartType enum. Encapsulates the object that represents charttype in Go.'
## ChartType Enum
Enumerates all chart types used in Excel.
```go
type ChartType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Area](./area/) | Represents Area Chart. |
|[AreaStacked](./areastacked/) | Represents Stacked Area Chart. |
|[Area100PercentStacked](./area100percentstacked/) | Represents 100% Stacked Area Chart. |
|[Area3D](./area3d/) | Represents 3D Area Chart. |
|[Area3DStacked](./area3dstacked/) | Represents 3D Stacked Area Chart. |
|[Area3D100PercentStacked](./area3d100percentstacked/) | Represents 3D 100% Stacked Area Chart. |
|[Bar](./bar/) | Represents Bar Chart: Clustered Bar Chart. |
|[BarStacked](./barstacked/) | Represents Stacked Bar Chart. |
|[Bar100PercentStacked](./bar100percentstacked/) | Represents 100% Stacked Bar Chart. |
|[Bar3DClustered](./bar3dclustered/) | Represents 3D Clustered Bar Chart. |
|[Bar3DStacked](./bar3dstacked/) | Represents 3D Stacked Bar Chart. |
|[Bar3D100PercentStacked](./bar3d100percentstacked/) | Represents 3D 100% Stacked Bar Chart. |
|[Bubble](./bubble/) | Represents Bubble Chart. |
|[Bubble3D](./bubble3d/) | Represents 3D Bubble Chart. |
|[Column](./column/) | Represents Column Chart: Clustered Column Chart. |
|[ColumnStacked](./columnstacked/) | Represents Stacked Column Chart. |
|[Column100PercentStacked](./column100percentstacked/) | Represents 100% Stacked Column Chart. |
|[Column3D](./column3d/) | Represents 3D Column Chart. |
|[Column3DClustered](./column3dclustered/) | Represents 3D Clustered Column Chart. |
|[Column3DStacked](./column3dstacked/) | Represents 3D Stacked Column Chart. |
|[Column3D100PercentStacked](./column3d100percentstacked/) | Represents 3D 100% Stacked Column Chart. |
|[Cone](./cone/) | Represents Cone Chart. |
|[ConeStacked](./conestacked/) | Represents Stacked Cone Chart. |
|[Cone100PercentStacked](./cone100percentstacked/) | Represents 100% Stacked Cone Chart. |
|[ConicalBar](./conicalbar/) | Represents Conical Bar Chart. |
|[ConicalBarStacked](./conicalbarstacked/) | Represents Stacked Conical Bar Chart. |
|[ConicalBar100PercentStacked](./conicalbar100percentstacked/) | Represents 100% Stacked Conical Bar Chart. |
|[ConicalColumn3D](./conicalcolumn3d/) | Represents 3D Conical Column Chart. |
|[Cylinder](./cylinder/) | Represents Cylinder Chart. |
|[CylinderStacked](./cylinderstacked/) | Represents Stacked Cylinder Chart. |
|[Cylinder100PercentStacked](./cylinder100percentstacked/) | Represents 100% Stacked Cylinder Chart. |
|[CylindricalBar](./cylindricalbar/) | Represents Cylindrical Bar Chart. |
|[CylindricalBarStacked](./cylindricalbarstacked/) | Represents Stacked Cylindrical Bar Chart. |
|[CylindricalBar100PercentStacked](./cylindricalbar100percentstacked/) | Represents 100% Stacked Cylindrical Bar Chart. |
|[CylindricalColumn3D](./cylindricalcolumn3d/) | Represents 3D Cylindrical Column Chart. |
|[Doughnut](./doughnut/) | Represents Doughnut Chart. |
|[DoughnutExploded](./doughnutexploded/) | Represents Exploded Doughnut Chart. |
|[Line](./line/) | Represents Line Chart. |
|[LineStacked](./linestacked/) | Represents Stacked Line Chart. |
|[Line100PercentStacked](./line100percentstacked/) | Represents 100% Stacked Line Chart. |
|[LineWithDataMarkers](./linewithdatamarkers/) | Represents Line Chart with data markers. |
|[LineStackedWithDataMarkers](./linestackedwithdatamarkers/) | Represents Stacked Line Chart with data markers. |
|[Line100PercentStackedWithDataMarkers](./line100percentstackedwithdatamarkers/) | Represents 100% Stacked Line Chart with data markers. |
|[Line3D](./line3d/) | Represents 3D Line Chart. |
|[Pie](./pie/) | Represents Pie Chart. |
|[Pie3D](./pie3d/) | Represents 3D Pie Chart. |
|[PiePie](./piepie/) | Represents Pie of Pie Chart. |
|[PieExploded](./pieexploded/) | Represents Exploded Pie Chart. |
|[Pie3DExploded](./pie3dexploded/) | Represents 3D Exploded Pie Chart. |
|[PieBar](./piebar/) | Represents Bar of Pie Chart. |
|[Pyramid](./pyramid/) | Represents Pyramid Chart. |
|[PyramidStacked](./pyramidstacked/) | Represents Stacked Pyramid Chart. |
|[Pyramid100PercentStacked](./pyramid100percentstacked/) | Represents 100% Stacked Pyramid Chart. |
|[PyramidBar](./pyramidbar/) | Represents Pyramid Bar Chart. |
|[PyramidBarStacked](./pyramidbarstacked/) | Represents Stacked Pyramid Bar Chart. |
|[PyramidBar100PercentStacked](./pyramidbar100percentstacked/) | Represents 100% Stacked Pyramid Bar Chart. |
|[PyramidColumn3D](./pyramidcolumn3d/) | Represents 3D Pyramid Column Chart. |
|[Radar](./radar/) | Represents Radar Chart. |
|[RadarWithDataMarkers](./radarwithdatamarkers/) | Represents Radar Chart with data markers. |
|[RadarFilled](./radarfilled/) | Represents Filled Radar Chart. |
|[Scatter](./scatter/) | Represents Scatter Chart. |
|[ScatterConnectedByCurvesWithDataMarker](./scatterconnectedbycurveswithdatamarker/) | Represents Scatter Chart connected by curves, with data markers. |
|[ScatterConnectedByCurvesWithoutDataMarker](./scatterconnectedbycurveswithoutdatamarker/) | Represents Scatter Chart connected by curves, without data markers. |
|[ScatterConnectedByLinesWithDataMarker](./scatterconnectedbylineswithdatamarker/) | Represents Scatter Chart connected by lines, with data markers. |
|[ScatterConnectedByLinesWithoutDataMarker](./scatterconnectedbylineswithoutdatamarker/) | Represents Scatter Chart connected by lines, without data markers. |
|[StockHighLowClose](./stockhighlowclose/) | Represents High-Low-Close Stock Chart. |
|[StockOpenHighLowClose](./stockopenhighlowclose/) | Represents Open-High-Low-Close Stock Chart. |
|[StockVolumeHighLowClose](./stockvolumehighlowclose/) | Represents Volume-High-Low-Close Stock Chart. |
|[StockVolumeOpenHighLowClose](./stockvolumeopenhighlowclose/) | Represents Volume-Open-High-Low-Close Stock Chart. |
|[Surface3D](./surface3d/) | Represents Surface Chart: 3D Surface Chart. |
|[SurfaceWireframe3D](./surfacewireframe3d/) | Represents Wireframe 3D Surface Chart. |
|[SurfaceContour](./surfacecontour/) | Represents Contour Chart. |
|[SurfaceContourWireframe](./surfacecontourwireframe/) | Represents Wireframe Contour Chart. |
|[BoxWhisker](./boxwhisker/) | The series is laid out as box and whisker. |
|[Funnel](./funnel/) | The series is laid out as a funnel. |
|[ParetoLine](./paretoline/) | The series is laid out as pareto lines. |
|[Sunburst](./sunburst/) | The series is laid out as a sunburst. |
|[Treemap](./treemap/) | The series is laid out as a treemap. |
|[Waterfall](./waterfall/) | The series is laid out as a waterfall. |
|[Histogram](./histogram/) | The series is laid out as a histogram. |
|[Map](./map/) | The series is laid out as a region map. |
|[RadialHistogram](./radialhistogram/) | The series is laid out as a radial historgram. It is used only for rendering |
