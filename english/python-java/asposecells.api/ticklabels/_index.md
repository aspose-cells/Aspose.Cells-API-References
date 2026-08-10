---
title: "TickLabels Class"
linktitle: "TickLabels"
articleTitle: "TickLabels"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the tick-mark labels associated with tick marks on a chart axis."
type: docs
weight: 6960
url: /python-java/asposecells.api/ticklabels/
---

## TickLabels class

Represents the tick-mark labels associated with tick marks on a chart axis.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Font](#font) | Font | Returns a Font object that represents the font of the specified TickLabels object. |
| [AutoScaleFont](#autoscalefont) | boolean | True if the text in the object changes font size when the object size changes. The default value is True. |
| [BackgroundMode](#backgroundmode) | int | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. |
| [RotationAngle](#rotationangle) | int | Represents text rotation angle in clockwise. 0: Not rotated. 255: Top to Bottom. -90: Downward. 90: Upward. |
| [IsAutomaticRotation](#isautomaticrotation) | boolean | Indicates whether the rotation angle is automatic |
| [NumberFormat](#numberformat) | String | Represents the format string for the TickLabels object. The formatting string is same as a custom format string setting  |
| [Number](#number) | int | Represents the format number for the TickLabels object. |
| [NumberFormatLinked](#numberformatlinked) | boolean | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the |
| [DisplayNumberFormat](#displaynumberformat) | String | Gets and sets the display number format of tick labels. |
| [Offset](#offset) | int | Gets and sets the distance between the axis labels and the axis line. The default distance is 100 percent, which represe |
| [TextDirection](#textdirection) | int | Represents text reading order. The value of the property is TextDirectionType integer constant. NOTE: This member is now |
| [ReadingOrder](#readingorder) | int | Represents text reading order. The value of the property is TextDirectionType integer constant. |
| [DirectionType](#directiontype) | int | Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant. |
| [TickLabelItems](#ticklabelitems) | TickLabelItem[] | Gets the display tick labels of the axis. Only available after calling Chart.calculate() method. |
| [AlignmentType](#alignmenttype) | int | Gets and sets the text alignment for the tick labels on the axis. The value of the property is TickLabelAlignmentType in |

### TickLabels.Font property {#font}

Returns a Font object that represents the font of the specified TickLabels object.

**Type:** Font

### TickLabels.AutoScaleFont property {#autoscalefont}

True if the text in the object changes font size when the object size changes. The default value is True.

**Type:** boolean

### TickLabels.BackgroundMode property {#backgroundmode}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.

**Type:** int

### TickLabels.RotationAngle property {#rotationangle}

Represents text rotation angle in clockwise. 0: Not rotated. 255: Top to Bottom. -90: Downward. 90: Upward.

**Type:** int

### TickLabels.IsAutomaticRotation property {#isautomaticrotation}

Indicates whether the rotation angle is automatic

**Type:** boolean

### TickLabels.NumberFormat property {#numberformat}

Represents the format string for the TickLabels object. The formatting string is same as a custom format string setting to a cell. For example, "$0".

**Type:** String

### TickLabels.Number property {#number}

Represents the format number for the TickLabels object.

**Type:** int

### TickLabels.NumberFormatLinked property {#numberformatlinked}

True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

**Type:** boolean

### TickLabels.DisplayNumberFormat property {#displaynumberformat}

Gets and sets the display number format of tick labels.

**Type:** String

### TickLabels.Offset property {#offset}

Gets and sets the distance between the axis labels and the axis line. The default distance is 100 percent, which represents the default spacing between the axis labels and the axis line. The value can be an integer percentage from 0 through 1000, relative to the axis label’s font size.

**Type:** int

### TickLabels.TextDirection property {#textdirection}

Represents text reading order. The value of the property is TextDirectionType integer constant. NOTE: This member is now obsolete. Instead, please use TickLabels.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### TickLabels.ReadingOrder property {#readingorder}

Represents text reading order. The value of the property is TextDirectionType integer constant.

**Type:** int

### TickLabels.DirectionType property {#directiontype}

Gets and sets the direction of text. The value of the property is ChartTextDirectionType integer constant.

**Type:** int

### TickLabels.TickLabelItems property {#ticklabelitems}

Gets the display tick labels of the axis. Only available after calling Chart.calculate() method.

**Type:** TickLabelItem[]

### TickLabels.AlignmentType property {#alignmenttype}

Gets and sets the text alignment for the tick labels on the axis. The value of the property is TickLabelAlignmentType integer constant.

**Type:** int
