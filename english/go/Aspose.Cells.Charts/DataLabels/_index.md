---
title: DataLabels Class 
linktitle: DataLabels
second_title: Aspose.Cells for Go API Reference
description: 'DataLabels class. Encapsulates the object that represents datalabels in Go.'
type: docs
weight: 200
url: /go/aspose.cells.charts/datalabels/
---

## DataLabels class

Encapsulates a collection of all the DataLabel objects for the specified Series.

```go

type DataLabels struct 

datalabels, _ := asposecells.NewDataLabels()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewDataLabels_DataLabels](./newdatalabels_datalabels/) | Constructs from an implementation object. | 
|[NewDataLabels_ChartTextFrame](./newdatalabels_charttextframe/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetBorder](./getborder/) | Gets the <see cref="Line">border</see>. | 
|[GetArea](./getarea/) | Gets the <see cref="Area">area</see>. | 
|[IsAutoText](./isautotext/) | Indicates the text is auto generated. | 
|[SetIsAutoText](./setisautotext/) | Indicates the text is auto generated. | 
|[GetDirectionType](./getdirectiontype/) | Gets and sets the direction of text. | 
|[SetDirectionType](./setdirectiontype/) | Gets and sets the direction of text. | 
|[GetText](./gettext/) | Gets or sets the text of data label. | 
|[SetText](./settext/) | Gets or sets the text of data label. | 
|[IsTextWrapped](./istextwrapped/) | Gets or sets a value indicating whether the text is wrapped. | 
|[SetIsTextWrapped](./setistextwrapped/) | Gets or sets a value indicating whether the text is wrapped. | 
|[GetBackgroundMode](./getbackgroundmode/) | Gets and sets the display mode of the background | 
|[SetBackgroundMode](./setbackgroundmode/) | Gets and sets the display mode of the background | 
|[GetShowValue](./getshowvalue/) | Represents a specified chart's data label values display behavior. True displays the values. False to hide. | 
|[SetShowValue](./setshowvalue/) | Represents a specified chart's data label values display behavior. True displays the values. False to hide. | 
|[GetShowCellRange](./getshowcellrange/) | Indicates whether showing cell range as the data labels. | 
|[SetShowCellRange](./setshowcellrange/) | Indicates whether showing cell range as the data labels. | 
|[GetShowPercentage](./getshowpercentage/) | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. | 
|[SetShowPercentage](./setshowpercentage/) | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. | 
|[GetShowBubbleSize](./getshowbubblesize/) | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. | 
|[SetShowBubbleSize](./setshowbubblesize/) | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. | 
|[GetShowCategoryName](./getshowcategoryname/) | Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide. | 
|[SetShowCategoryName](./setshowcategoryname/) | Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide. | 
|[GetShowSeriesName](./getshowseriesname/) | Indicates whether the series name displays for the data labels on a chart.True to show the series name. False to hide. | 
|[SetShowSeriesName](./setshowseriesname/) | Indicates whether the series name displays for the data labels on a chart.True to show the series name. False to hide. | 
|[GetShowLegendKey](./getshowlegendkey/) | Represents a specified chart's data label legend key display behavior.True if the data label legend key is visible. | 
|[SetShowLegendKey](./setshowlegendkey/) | Represents a specified chart's data label legend key display behavior.True if the data label legend key is visible. | 
|[Get_NumberFormat](./get_numberformat/) | Represents the format string for the DataLabels object. | 
|[SetNumberFormat](./setnumberformat/) | Represents the format string for the DataLabels object. | 
|[GetNumber](./getnumber/) | Gets and sets the built-in number format. | 
|[SetNumber](./setnumber/) | Gets and sets the built-in number format. | 
|[GetNumberFormatLinked](./getnumberformatlinked/) | True if the number format is linked to the cells(so that the number format changes in the labels when it changes in the cells). | 
|[SetNumberFormatLinked](./setnumberformatlinked/) | True if the number format is linked to the cells(so that the number format changes in the labels when it changes in the cells). | 
|[ApplyFont](./applyfont/) | Apply the font of the datalabels to all child nodes. | 
|[GetFont](./getfont/) | Gets the font of the DataLabels; | 
|[GetSeparatorType](./getseparatortype/) | Gets or sets the separator type used for the data labels on a chart. | 
|[SetSeparatorType](./setseparatortype/) | Gets or sets the separator type used for the data labels on a chart. | 
|[GetSeparatorValue](./getseparatorvalue/) | Gets or sets the separator value used for the data labels on a chart. | 
|[SetSeparatorValue](./setseparatorvalue/) | Gets or sets the separator value used for the data labels on a chart. | 
|[GetPosition](./getposition/) | Represents the position of the data label. | 
|[SetPosition](./setposition/) | Represents the position of the data label. | 
|[IsNeverOverlap](./isneveroverlap/) | Indicates whether the datalabels display never overlap. (For Pie chart) | 
|[SetIsNeverOverlap](./setisneveroverlap/) | Indicates whether the datalabels display never overlap. (For Pie chart) | 
|[GetShapeType](./getshapetype/) | Gets or sets  shape type of data label. | 
|[SetShapeType](./setshapetype/) | Gets or sets  shape type of data label. | 
|[IsDeleted](./isdeleted/) | Indicates whether this data labels is deleted. | 
|[SetIsDeleted](./setisdeleted/) | Indicates whether this data labels is deleted. | 
|[GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Gets and sets the text horizontal alignment. | 
|[SetTextHorizontalAlignment](./settexthorizontalalignment/) | Gets and sets the text horizontal alignment. | 
|[GetTextVerticalAlignment](./gettextverticalalignment/) | Gets or sets the text vertical alignment of text. | 
|[SetTextVerticalAlignment](./settextverticalalignment/) | Gets or sets the text vertical alignment of text. | 
|[GetRotationAngle](./getrotationangle/) | Represents text rotation angle. | 
|[SetRotationAngle](./setrotationangle/) | Represents text rotation angle. | 
|[IsAutomaticRotation](./isautomaticrotation/) | Indicates whether the text of the chart is automatically rotated. | 
|[Characters](./characters/) | Returns a Characters object that represents a range of characters within the text. | 
|[GetReadingOrder](./getreadingorder/) | Represents text reading order. | 
|[SetReadingOrder](./setreadingorder/) | Represents text reading order. | 
|[IsResizeShapeToFitText](./isresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting iswhen text within a shape is scaled in order to contain all the text inside. | 
|[SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting iswhen text within a shape is scaled in order to contain all the text inside. | 
|[GetLinkedSource](./getlinkedsource/) | Gets and sets a reference to the worksheet. | 
|[SetLinkedSource](./setlinkedsource/) | Gets and sets a reference to the worksheet. | 
